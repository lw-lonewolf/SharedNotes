f## Affordances 
Affordances refer to the actual and perceived properties of an object that determine exactly how it can be used. 

**Perceivibility:**
If a user looks at an object and immediately knows how it can be used they have successfully perceived its affordances.

* **Manual Affordances:** This refers to the natural way of human understanding of how physical objects are manipulated in real life. e.g. recognizing "pushable" objects. 
* **Virtual vs. Physical:** While physical inspection of an object (like a saw) reveals it purpose, virtual object representations are often less recognizable. e.g. users expect a digital button to change visually when "pushed" to confirm this interaction.

##### Affordance Matrix
* *Perceptible Affordance:* Actual properties match perceptual information
* *False Affordance:* Perceptual information suggests an affordance that does not exist. (Button has hints that it sinks when pushed "but doesn't sink")
* *Hidden Affordance:* A property exists but isn't perceived by the user.
* *Correct Rejection:* No affordance exists and no perceptual information suggests this. 


## Constraints
Visible Limitations that restrict the range of possible actions perceived by the user. 

* A physical example of this would be a door with a metallic plate. (this means the door is pushable only, not to be pulled.). On the other hand a handle would mean the door may be pullable/turnable.

* Another example would be a pair of scissors with two holes, one bigger hole for multiple fingers and a smaller one for the thumb. This way it constrains the user forcing him/her to hold it correctly with the correct grip.

## Mapping
Mapping is the relationship between controls and their actions or the parts they operate.

The goal of good mapping is that how things should work is apparent to the user through the visual layout. 

e.g. There is a direct mapping between the holes and the fingers intended to operate them. (Scissors)

***Failure of Mapping (Digital Watches)***
A digital watch has four buttons (controls) with high affordance (clearly pushable) but what they do is NOT apparent (unknown mapping and constraints). Because there is no visible relation between buttons and end results. The functions are not intuitive and must be taught.
#### Types of Mapping
* *Physical Mapping*
	`Covered Above`
* *Control to Result Mapping*
	The relationship between a controls movement and the resulting change, e.g. slider to change brightness/volume (right increases, left decreases).
* *Spatial Mapping*
	This occurs when digital layout mirrors a physical arrangement 

# DETAILED EXAMPLE
A highly detailed example of a software system to illustrate these concepts is the **SecureBank TellerStation**, a **sovereign desktop application**. Designed for "perpetual intermediates," it uses a **minimal visual style** to prevent fatigue during long work shifts.

Below is a highlight of every type of affordance, constraint, and mapping within this system, drawing from the principles in the sources:

### **1. Affordances**

Affordances are the perceived and actual properties of the software that determine how it can be used.

- **Manual Affordances**: The physical keyboard and mouse used by the bank teller are "manual affordances." The teller inherently understands these are for typing data and pointing at elements on the screen through hand manipulation.
- **Virtual Affordances**: On the screen, a "New Account" button is rendered with a 3D-dimensional bevel. This visual property makes the button look "pushable," creating a digital expectation that it will react when clicked.
- **Perceptible Affordance**: When the teller sees a "Print Receipt" button and clicks it, the actual property (printing) matches the perceptual information (the icon and label). This is a successful, honest interaction.
- **False Affordance (Bait-and-Switch)**: The application features a "Save" icon (a floppy disk). However, clicking it actually opens a "Search" menu. This is a **"bait-and-switch manual affordance"** because the program fails to deliver on the expectation it set.
- **Hidden Affordance**: In the transaction ledger, a teller can double-click a row to see a hidden audit log. However, there is no visual clue (like an icon or highlight) that this action is possible. The property exists, but it is not perceptible.
- **Correct Rejection**: A button labeled "Delete Branch History" is grayed out and flat. It does not look clickable, and it has no actual function for a standard teller. The teller correctly perceives that no interaction is possible.

### **2. Constraints**

Constraints are **visible limitations** that restrict the range of possible actions, helping the teller avoid errors.

- **GUI Constraints**: In the "Deposit Amount" field, the software only allows the entry of numbers and a single decimal point. By physically preventing the teller from typing letters or symbols, the interface limits the usage possibilities to valid data only.
- **Action Constraints**: The "Approve Loan" button is invisible unless the teller has logged in with "Manager" credentials. This directly restricts the actions possible based on the user's role and the application's current state.

### **3. Mapping**

Mapping is the relationship between the controls provided and the resulting actions or the parts of the system they operate.

- **Control-to-Result Mapping**: To adjust the brightness of the ledger display, the teller uses a horizontal slider. Moving the slider to the right (up) to increase brightness and to the left (down) to decrease it provides a clear **relationship between the control and the result**.
- **Spatial Mapping**: The digital representation of the teller’s "Cash Drawer" on the screen is arranged in a layout that mirrors the physical drawer in front of them. The top-left digital slot operates the top-left physical bin, making the **implications of how the operating parts work clear**.
