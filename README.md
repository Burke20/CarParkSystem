# Car Park Sensor System  

## This is my Project for IoT Standards and Protocols  

### What is the Project About?  
My proposed project is to create a **sensor system for a car park**, such as the **SETU Waterford campus car park**.  
- The system will be installed in each parking space.  
- At each entrance, it will display whether the **car park is full or not**.  
- Each parking spot will have a **red or green light** to indicate availability, helping drivers navigate efficiently.  

### Why Did I Choose This Idea?  
I chose this idea because **finding parking in college has been a challenge**.  
- Many students and lecturers drive into the campus only to find no spaces available, causing them to **miss their lectures**.  
- Having an **indicator at the entrance** would help drivers decide whether to enter or park elsewhere, saving time.  
- While similar systems exist, **I haven’t seen this on a smaller, private scale**, and I believe recreating this technology would be valuable.  
- It could also serve as a **future idea for the college to implement**.  

### How Will I Implement This?  
I will use:  
- A **Raspberry Pi** (provided).  
- **Included sensors** (motion & light sensor).  
- **Azure** and relevant IDE(s) to configure **MQTT communication**.  
- A **Python script** to:  
  - Collect and process sensor data.  
  - Display the parking status on an **easy-to-read interface**.  

### What Sensors and Why?  
I have chosen to use **two sensors**:  

1. **Motion Sensor**  
   - Detects movement in a parking space.  
   - **Triggers the parking script** to start checking for occupancy.  

2. **Light Sensor**  
   - Measures light levels in the parking spot.  
   - Ensures the detected motion was actually a **car**, not a bird or a pedestrian.  

**Why Two Sensors?**  
- Using **two metrics** ensures **accuracy** before marking a spot as **occupied**.  
- The **motion sensor** activates the process, and the **light sensor** confirms vehicle presence.  

### What is the Data Visualisation/Response?  
- The **Python script** will:  
  1. Run a **check** to verify that the detected object is a car.  
  2. If the check **passes**, the system will **record data in real time**.  
  3. The data will indicate whether a **parking spot is occupied or empty**.  
  4. When the sensors reach a **certain threshold**, the status of the spot will update accordingly.  

**Indicator System**:  
- **Red light** = Parking spot **occupied**.  
- **Green light** = Parking spot **available**.  

This system will provide **real-time updates** to help **optimize parking efficiency** on campus.  

### What Response and Actuations Will Be Triggered?  
- The **user/data analyst** will be able to:  
  - See whether each spot is **full or empty**.  
  - Track how long a car has been parked to detect **overstayed vehicles**.  
  - Identify the **individual spot number** for advanced tracking.  
  - Use **data analysis** to determine the **best entrance for directing traffic**, based on available spaces in each area.  

- **Physical Actuation**:  
  - A **light will change color** based on the parking spot status:  
    - **Red light** = Spot is **occupied**.  
    - **Green light** = Spot is **available**.  

### Summary  
To summarise, I am confident that this project will be a **great demonstration of real-world IoT applications**, using:  
- **Sensors**  
- **Python scripts**  
- **A compatible IDE**  
- **Azure with MQTT Communication**  

I look forward to **starting development and keeping this repository updated with progress!** 
