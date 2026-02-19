This is not a UML diagram. its idea is to put the entire system into an understandable context and highlight how the high level components are related to each other.
###### Superordinate 
* tells what systems your system talks to
###### Subordinate
* receives information 
###### Peer 
Shares info to and from. 
## Styles of Arrow and Box Diagram
There are many styles of an arrow and box diagram, its *not a UML diagram.* *We use box and arrows*
### Data Flow Diagram 
![[Data Flow ArCD]]
These perform **processing**. The *boxes are filters* and arrows transfer information and are called *pipes*. This architecture is used for example in image processing or compilers. 
##### Special Case: Batch Sequential 
![[Architecture Introduction 2025-06-01 18.04.50.excalidraw]]
### Data Centred Diagram 
* They store and retrieve component from a repository. 
* Act just like an Observer design pattern, if repository state changes tell all Cs 
* As many computing components as required can be added. 
* Has very low coupling 
* Disadvantage: if data source fails the whole system fails. 
 ![[Architecture Introduction 2025-06-01 18.08.32.excalidraw]]
##### Special Case: Clients & Server
Self explanatory
#### Layered architecture
* coupling is contained 
* the OSI model is an exampled of layered architecture
* When security is important we use layers 
* if availability is important, we introduce redundancy (have multiple servers)
![[Architecture Introduction 2025-06-01 18.15.55.excalidraw]]
#### Object Oriented 
![[Architecture Introduction 2025-06-01 18.17.04.excalidraw]]
The *Cs* here are actual Classes
#### Call & Return
![[Architecture Introduction 2025-06-01 18.19.19.excalidraw]]
* The arrows going **downwards** specify *calls* while the one going upwards are *returns*
* The reason this is different from the other architectures is that the boxes are not at the same level of abstraction. Going downwards the level of abstraction decreases. The decision makers are at the top and the works are at the bottom. 
