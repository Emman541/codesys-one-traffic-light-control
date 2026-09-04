# codesys-one-traffic-light-control
PLC-based traffic light control system simulated in CODESYS using Structured Text and Visualization.
# 🚦 CODESYS Traffic Light Control System

A PLC-based traffic light control system developed and simulated using **CODESYS** and **Structured Text (ST)**.

The project demonstrates basic PLC sequencing, timer control, state machines, and HMI-style visualization.

## 🎯 Project Objective

The objective of this project is to simulate a simple traffic light system where the lights automatically transition through:

**Green → Yellow → Red → Green**

The system was developed to strengthen my understanding of PLC programming and industrial automation.

## 🛠️ Technologies Used

* CODESYS
* Structured Text (ST)
* PLC Timers
* State Machine Logic
* CODESYS Visualization

## ⚙️ How It Works

The traffic light operates using a state-based control system.

| State   | Light     |
| ------- | --------- |
| State 1 | 🟢 Green  |
| State 2 | 🟡 Yellow |
| State 3 | 🔴 Red    |

Timers control how long each state remains active before the system transitions to the next state.

## 🧠 Control Logic

The system uses a `CASE` statement to control the different traffic-light states.

Example:

```text
CASE iState OF

    1:
        Green := TRUE;
        Yellow := FALSE;
        Red := FALSE;

    2:
        Green := FALSE;
        Yellow := TRUE;
        Red := FALSE;

    3:
        Green := FALSE;
        Yellow := FALSE;
        Red := TRUE;

END_CASE;
```

Timers are used to determine when the controller should move from one state to another.

## 🖥️ Visualization

The traffic light was also visualized in CODESYS to provide a simple graphical representation of the PLC outputs.

### Traffic Light Visualization

![Traffic Light](screenshots/traffic-light.png)

## 📚 What I Learned

Through this project, I practiced:

* Structured Text programming
* PLC state machines
* TON timers
* Boolean variables
* Sequential control
* CODESYS visualization
* Basic HMI concepts
* Connecting PLC logic to visualization objects

## 🚀 Future Improvements

Planned improvements include:

* [ ] Two-way traffic intersection
* [ ] Pedestrian crossing
* [ ] Four-way intersection
* [ ] Vehicle simulation
* [ ] Emergency vehicle priority
* [ ] More advanced traffic management logic

## 👨🏽‍💻 Author

**Emmanuel Faparusi**

Mechatronics Engineering | Embedded Systems • Automation • IoT

