The core design principle behind design principles is that no matter how "cute" or "visually pleasing" an app is. It'll be irritative/hard to use unless it acts like a "fellow worker" for the user instead of a software that is very picky about how it receives information or if it forces the user to hunt down for a commonly used feature. There are a number of key features that should be present in a software 

* ***Take an Interest (Memory)***
	A considerate e-commerce site would remember a user's name and address after the first entry instead of having them re-enter it every time.
* ***Be Forthcoming***
	The product should provide information regarding the user's goals. e.g. if the printer is about to be empty, send a notification about low paper supplies, instead of just waiting for a printer failure.
* ***Use Common Sense***
	Designers must avoid placing harmless, frequently used functions immediately adjacent to harmful or "ejector seat" expert functions. A bad example of this would be having the "Unmount" and "Format Disk" options right next to each other in a disk management app.
* ***Be Conscientious***
	The app should be "OCD" about details, ensure checks for details repeatedly, e.g. verifying no file exists with the same name before accepting a new file name.
* ***Don't Burden the User with Personal Problems***
	Software should not "whine" to the user about its problems, with error messages or prompts such as "document successfully autosaved"
* ***Don't ask a lot of questions***
	Bad example: 
	Enter File Name -> Click Save -> "Are you sure you want to save?"
	-> "Click Yes" 
* ***Be Perceptive***
	Watch user preferences and remember without asking. e.g. If user sets font to "Times New Roman", inserting a new text box should not default to the original one, instead it should remember Times New Roman.
* ***Fail Gracefully***
	Do not just go ahead and crash with zero errors or reasons. Another thing would be if a user is filling a form and some entries are incorrect or have errors, DO NOT REMOVE ALL ENTRIES ON REJECTION instead only highlight the wrong ones. 
* ***Help Avoid Awkward Mistake***
	e.g. Warn the user he is about to send an email without a subject. 

#### A "SMART" Product
A smart product is one that has a memory, anticipates needs, and remembers details like past file locations, or past date entries, last used font etc. 

>[!NOTE] Fundamental Rule for Smart Products
> If it's worth it to the user, it's worth it to the application to remember it. 


##### Designing Social Applications 
Social Products must navigate more restrictions e.g. social norms (unspoken rules of reciprocity and gratitude) and market norms(business deals involving fair price and honesty). Key considerations would involve: 

* **Identity and Profiles:** Users should have complete control over their profiles and who can see their information. 
* **Collaboration:** Products should permit easy collaboration, such as threading comments in Google Documentation
* **Shutting the Door:** A polite way to suspend social interruptions when working. (DND mode on discord etc.)
* **Handling Griefers:** Application should be capable of recognizing and appropriately deal with people trying to ragebait other people.
* **Respecting Privacy:** Designers must resist the strong financial benefits in invading user's privacy.



### **Scenario: The "TeamFlow" Redesign**

**1. Taking an Interest and Having a Memory** TeamFlow's old version required users to re-select their department and active project every time they logged in. According to the sources, software should **work hard to remember our habits**. In the redesign, TeamFlow now **takes an interest** by remembering Alex's previous view and automatically launching to his **last active project position**, behaving like a supportive human colleague who knows your current focus.

**2. Being Forthcoming and Keeping the User Informed** When Alex clicks to generate a massive quarterly report, a **forthcoming** product provides information related to his goals. Instead of just showing a generic progress bar, TeamFlow informs him that the company's shared printer is currently out of paper or that there is a long queue, allowing him to pivot his tasks rather than waiting for a failure.

**3. Using Common Sense** The designers noticed that the "Complete Project" button (an irreversible expert function) was right next to the "Add Task" button (a frequent activity). Following the principle of **common sense**, they moved these controls apart to prevent accidental "ejector-seat" activations.

**4. Failing Gracefully** Alex fills out an 11-field project initiation form. Due to a momentary server drop, the submission fails. Rather than forcing him to click the "Back" arrow only to find **all valid entries discarded**, TeamFlow **fails gracefully** by caching his input locally and allowing him to re-submit once the connection is restored.

**5. Avoiding Awkward Mistakes** Alex attempts to send a project update to "The Board" group. TeamFlow notices he mentions an "attached budget" in his text but hasn't attached a file. It **perceptively** flags this, helping him **avoid an awkward mistake** and earning his trust rather than berating him with an error message later.

**6. Smart Behavior: Putting Idle Cycles to Work** While Alex is reading a document, TeamFlow doesn't remain idle. It uses **idle cycles** to proactively index his new tasks and **anticipate his needs** by pre-loading the most likely next files he will need based on his **characteristic patterns**.

**7. Not Burdening the User with Personal Problems** The sources state that users do not need to see technical details like **data transfer rates or loading sequences**. When TeamFlow syncs with the cloud, it does so quietly in the background without **"whining"** at Alex with confirmation dialog boxes like "Sync Successful" for every minor update.

**8. Being Perceptive with Preferences** Alex prefers a specific font size for his dashboard. Rather than requiring him to manually set this every run—which **mainstream applications** often do—TeamFlow **watches his preferences** and adopts them as the new standard, realizing that **if it is worth it to the user to do, it is worth it to the application to remember**.

---

**Analogy for Understanding:** A **considerate product** is like a **seasoned executive assistant**: they have your favorite coffee ready before you ask (Perceptive), they don't interrupt your meeting to tell you they finished filing papers (Not burdening you with personal problems), and they quietly catch you at the door if you've forgotten your briefcase (Helping avoid awkward mistakes). An **inconsiderate product** is like a **temp worker** who asks for your name every morning, interrupts you to announce every small task they complete, and throws away your entire project if they find one single typo.