## Pattern Name and Classification 
-> Singleton *Object Creational*
## Intent
Ensure a class has only one instance, and provide a global point of access to it. 
## Motivation 
Its important for some classes to have exactly one instance. Although there can be many printers in a system, there should be only one printer spooler. There should be only one file system, and only one window manager etc. 
## Applicability 
Used when: 
* There must be exactly one instance of a class, and it must be accessible to clients from a well known access point. 
* When the sole instance should be extensible by subclassing, and clients should be able to use an extended instance without modifying their code. 
## Structure 
![[Singleton CD.png]]

## Participants 
* Singleton: defines an Instance operation that lets clients access its unique instance. Instance is a class operation (static member function in C++).
## Consequences
*  Controlled access to sole instance.
*  Reduced name space
*  Permits refinement of operations and representation
*  Permits a variable number of instances.
*  More flexible than class operations

## Implementation
```cpp
class Singleton{
public: 
	static Singleton* Instance(); 
protected: 
	Singleton(); 
private: 
	static Singleton* _instance;
}
```
```cpp
Singleton* Singleton::_instance = nullptr;
Singleton* Singleton::Instance() {
	if(_instance == nullptr){
		_instance = new Singleton;
	}
	return _instance;
}
```

## Sample Code 
Suppose we define a *MazeFactory* class for building mazes. 

```cpp
class MazeFactory{
public: 
	static MazeFactory* Instance(); 
	//existing interface comes here 
protected: 
	MazeFactory(); 
private: 
	static MazeFactory* _instance;
}
```
with the following implementation 
```cpp
MazeFactory* MazeFactory::_instance = nullptr; 
MazeFactory* MazeFactory::Instance(){
	if(_instance == 0){
		_instance = new MazeFactory;
	}
	return _instance;
}
```

If there were subclasses of *MazeFactory*, and the app must decide which to use, We'll select the kind of maze through an environment variable and add code. 
```cpp
MazeFactory* MazeFactory::Instance(){
	if(_instance == 0){
		const char* mazeStyle = getenv("MAZESTYLE");
		if (strcmp(mazeStyle, "bombed") == 0){
			_instance = new BombedMazeFactory;
		}
		//other sub classes 
		else {
			_instance = new MazeFactory;
		}
	}
	return _instance
}
```