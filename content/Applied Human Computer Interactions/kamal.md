## 🧩 **Case Study 4: Fitness Tracker App**

**Scenario:**  
Your company is developing a **fitness tracker app** that targets working adults who want to stay healthy despite busy schedules. The app should monitor daily steps, calories, heart rate, and sleep.

**Questions:**  
a) Identify the primary and secondary personas.  
b) Describe one key scenario for the app.  
c) Using Goal-Directed Design, explain how personas guide the interface design.  
d) Define one design requirement for the “Sleep Tracking” feature.  
e) Describe the interaction framework for viewing weekly fitness summary.

---

**Model Answers:**  
**a)**

- **Primary Persona:** _Sara, 28, Marketing Executive_ — wants to maintain fitness with minimal time. Frustration: complex menus.
    
- **Secondary Persona:** _Bilal, 35, Gym Enthusiast_ — wants detailed analytics and progress graphs. Frustration: lack of accuracy in data.
    

**b)**

> Sara wakes up, checks her “Daily Summary,” and sees she only completed 70% of her step goal yesterday. The app suggests a quick 15-minute walking plan for lunch break. She accepts, and the app schedules a reminder for noon.

**c)**

- Sara’s need for simplicity → dashboard with a single daily goal card.
    
- Bilal’s need for analytics → an optional “Insights” tab for in-depth graphs.
    
- Both personas push for a **tiered interface**: essential info first, advanced data deeper.
    

**d)**  
**Requirement:** The app must automatically detect sleep start and end times and display duration, quality (deep/light), and daily sleep consistency.

**e)**  
**Interaction Framework:**

- **Main screen:** Overview with 3 tiles (Steps, Calories, Sleep).
    
- **Weekly Summary:** Horizontal bar chart + average score.
    
- **Navigation:** _Home → Summary → Detail View → Back._
    
- Tooltip on each bar shows daily total; color-coded performance.
    

---

## 🧩 **Case Study 5: Library Management Kiosk**

**Scenario:**  
A university library is introducing **self-service kiosks** where students can borrow, return, and search for books without staff assistance.

**Questions:**  
a) Identify two personas.  
b) Describe one key scenario for borrowing a book.  
c) Define two design requirements for usability.  
d) Describe how the “what” of interaction design is represented here.

---

**Model Answers:**  
**a)**

- **Primary Persona:** _Hassan, 20, Undergraduate Student_ — Goal: borrow books quickly between classes. Frustration: long queues.
    
- **Secondary Persona:** _Ms. Rukhsana, 45, Librarian_ — Goal: reduce workload by monitoring kiosks remotely.
    

**b)**

> Hassan walks to the kiosk, scans his student card, types “Database Systems,” and taps “Borrow.” The kiosk displays location “Shelf C2,” he collects the book, and scans it again to confirm checkout.

**c)**

- **R1:** The kiosk shall complete the entire borrowing process in ≤ 4 steps.
    
- **R2:** Provide text-to-speech and large button options for accessibility.
    

**d)**  
The “what” focuses on enabling _self-service borrowing_, _search_, and _return_ tasks — not on how the backend RFID or UI animation works.

---

## 🧩 **Case Study 6: Online Food Ordering Platform**

**Scenario:**  
A food delivery startup wants to redesign its app to increase repeat orders and customer satisfaction.

**Questions:**  
a) Create a primary persona.  
b) Write one narrative/scenario for reordering past meals.  
c) Define two requirements derived from that scenario.  
d) Sketch an interaction framework for the “Reorder” feature.

---

**Model Answers:**  
**a)**  
**Primary Persona:** _Taha, 27, Office Worker_ — Orders lunch daily, prefers quick checkout, dislikes repetitive form-filling.

**b)**

> Taha opens the app, taps “Order History,” selects “Monday Lunch,” and taps “Reorder.” The system auto-fills address, payment, and delivery time. He confirms and gets an estimated delivery of 25 minutes.

**c)**

- **R1:** The system shall allow users to reorder previous meals with one tap.
    
- **R2:** The system shall automatically prefill delivery and payment details.
    

**d)**  
**Interaction Framework:**

- **Tabs:** _Home_, _Search_, _Order History_, _Profile_.
    
- **Flow:** _Order History → Select Order → Review → Confirm_.
    
- Confirmation toast + live tracking screen shown after checkout.
    

---

## 🧩 **Case Study 7: Smart Parking System**

**Scenario:**  
A city introduces a **smart parking app** that lets drivers locate and reserve parking spots in real time.

**Questions:**  
a) Define two personas.  
b) Describe one scenario showing parking reservation.  
c) Write one use case and one design requirement.  
d) Explain how user goals influence interface design.

---

**Model Answers:**  
**a)**

- **Primary Persona:** _Usman, 31, Salesman_ — drives daily to meetings, wants to find quick parking.
    
- **Secondary Persona:** _Aisha, 40, Working Mother_ — uses app occasionally, needs accessible spots close to elevators.
    

**b)**

> Usman enters the city, opens the app, and selects “Find Parking Near Me.” The app shows nearby spots on a map. He taps one labeled “Available — 150m away,” reserves it, and gets a timer and navigation link.

**c)**

- **Use Case:** User selects parking spot → system reserves it → timer starts → spot marked as occupied.
    
- **Requirement:** The system shall display real-time availability and allow 15-minute reservation holds.
    

**d)**  
User goals (speed, convenience, accessibility) guide the design — e.g., large map view, one-tap reservation, color-coded availability, and audible confirmation for accessibility.

---

## 🧩 **Case Study 8: Online Appointment Booking System**

**Scenario:**  
A hospital wants to build an **online appointment booking system** for patients to schedule and track medical visits.

**Questions:**  
a) Identify the primary persona and her motivation.  
b) Write a short scenario describing appointment scheduling.  
c) State two design requirements.  
d) Describe the interaction framework for managing appointments.

---

**Model Answers:**  
**a)**  
**Primary Persona:** _Dr. Maria, 34, Working Mother_ — wants to book doctor appointments for herself and her kids without phone calls or waiting lines.

**b)**

> Maria opens the app, taps “Book Appointment,” selects _Pediatrician → Next Available Slot → Tuesday 3 PM_. The system confirms and adds it to her calendar.

**c)**

- **R1:** The app shall show available doctors and time slots in a single view.
    
- **R2:** The app shall send appointment reminders 24 hours before the visit.
    

**d)**  
**Interaction Framework:**

- **Tabs:** _Home_, _Doctors_, _Appointments_, _Profile_.
    
- **Flow:** _Doctors → Select → Choose Slot → Confirm_.
    
- Calendar integration and “Reschedule” option in appointment details.