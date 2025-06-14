---
{"dg-publish":true,"permalink":"/general/team-terminology-glossary/"}
---

# General
### Preliminary Design Review (PDR)
A PDR serves as a first step to showing other people on the team the work you've been doing on your project and to discuss your steps moving forward. Ideally PDR's are done early in the design process to prevent having to backtrack. A subteam lead will help arrange a meeting so all relevant parties can give feedback on the work you've done and point out their unique needs from the project. After completing a PDR, work will continue until the project is ready for a [[General/Team Terminology (Glossary)#Design Review (DR)\|DR]].
### Design Review (DR)
A DR is the next step after a [[General/Team Terminology (Glossary)#Preliminary Design Review (PDR)\|PDR]]. At this stage the project should be near completion and feedback should be finishing touches before manufacturing begins. The presentation aspect is similar to the PDR, just naturally more developed.
### Drive Critical
Any portion of the car which, in its absence, would make the car undriveable. This could be for logistical reasons or safety reasons. For example, the motor is drive critical because it generates the force that moves the car; this is a logistical reason. On the other hand the [[General/Team Terminology (Glossary)#Shutdown Circuit\|shutdown circuit]] is drive critical because without it driving the car would be unsafe; this is a safety reason.
# Electrical
### Tractive System (TS)
By **EV.1.1**: "Every part electrically connected to the Motor(s) and/or Accumulator(s)"
### Grounded Low Voltage (GLV)
By **EV.1.2**: "Every electrical part that is not part of the Tractive System" More rules found in **EV.4.4** - must be Grounded to the Chassis and able to operate with the [[General/Team Terminology (Glossary)#Accumulator\|Accumulator]] removed from the vehicle
### Accumulator
By **EV.1.3**: "All the battery cells or super capacitors that store the electrical energy to be used by the Tractive System" More rules found in **EV.5.1**
### Penthouse
This is an internal term which describes the upper portion of our Accumulator container. We make this distinction as the [[Car Architecture#Penthouse\|penthouse]] contains the logic portion of the Accumulator, whereas we refer to the portion which contains the battery cells as simply the Accumulator. ==*By rules the penthouse is indistinguishable from the Accumulator*==
### Energy Meter
Described in **EV.3.2**: Measures power and voltage of the accumulator to ensure [[General/FSAE 2025 Rules\|rules]] compliance to **EV.3.3**
### Motor Controller / Inverter
Supplies power from the [[General/Team Terminology (Glossary)#Accumulator\|Accumulator]] to the motor. Converts DC to AC and regulates how much power goes to the motor based on a number of conditions, including torque requests from the [[Electrical/Drivetrain Electronics/ECU/ECU\|ECU]].
### Accelerator Pedal Position Sensor (APPS)
Described in **T.4.2**: Measures how far the accelerator pedal is depressed in order to determine how much power should go to the motor.
### Brake System Encoder (BSE)
Described in **T.4.3**: Measures brake system pressure.
### Maintenance Plugs
Described by **EV.5.3**: Electrically connects and disconnects [[General/Team Terminology (Glossary)#Accumulator\|Accumulator]] segments from one another for maintenance.
### Isolation Relays (IR)
Described by **EV.5.4**: Normally open relays which disconnect the two poles of the [[General/Team Terminology (Glossary)#Accumulator\|Accumulator]] and prevent High Voltage **T.9.1.1** from being present outside the Accumulator container.
### Manual Service Disconnect (MSD)
By **EV.5.5** "A Manual Service Disconnect (MSD) must be included to quickly disconnect one or the two poles of the Accumulator **EV.11.3.2**"
### Shutdown Circuit
The shutdown circuit (Described in [[General/FSAE 2025 Rules\|EV.7.2]]) is a safety mechanism which serves to disconnect the [[General/Team Terminology (Glossary)#Tractive System (TS)\|Tractive System]] either automatically or manually. This is done through a series of switches and [[General/Team Terminology (Glossary)#Interlocks\|interlocks]] which can break power supply to the [[General/Team Terminology (Glossary)#Isolation Relays (IR)\|IR'S]] thus isolating the Tractive System from the outside world to protect us from the high voltage. For specifics on the wiring, see the [[Car Architecture#Shutdown Circuit\|car architecture]].
### Interlocks
Described in **EV.7.8**: Interlocks are wires or connections which when unplugged open the shutdown circuit. Think of it like a safety switch which detects whether or not a plug is plugged in. They are required on the [[General/Team Terminology (Glossary)#Manual Service Disconnect (MSD)\|MSD]] and on any [[General/Team Terminology (Glossary)#Tractive System (TS)\|TS]] connector outside of a housing (including those that are mounted on a housing).
### Battery Pack Configuration Shorthand
Often it is helpful to know how many series and parallel connections a battery pack has. The number of series connections indicates the pack voltage, and the number of parallel connections indicates the pack current/capacity. To quickly share this information we use the shorthand "`XsYp`" where "`X`" denotes the number of series connections and "`Y`" the number of parallel connections. Meaning `10s4p` would represent a battery pack with `10` series connections and `4` parallel connections.
### Bus Load
The amount of information being sent over a communication bus. Based on the communication rate of the bus, there is an upper limit to the bus load which increases with communication rate. However, higher data transmission rates generally introduce more complications.
# Mechanical
🚧Under [[General/How to contribute to the megathread\|construction]]🚧