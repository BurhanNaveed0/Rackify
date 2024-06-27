## Rackify 🚲

A prototype bike racking system allowing users to pay to access bikes racks distributed across major cities via mobile app or pre-paid card. 
Achieved 3rd place overall at NJIT’s spring 2024 IEEE Hardware Hackathon, winning a $500 cash prize.

Team Members: Burhan Naveed, Matthew Levine, Prabhav Sharma, Tanush Tammanagoudar, Raghav Bharath

## Project Status ✔
Hackathon project complete. Post competition finishing touches in development:

- Transferring mock HTML mobile app to React Native for demoing on Expo.
- Adding user Authentication with Firebase.
- Handling rack occupation data in Firebase.

## Project Photos 📸

![cad](https://github.com/BurhanNaveed0/Rackify/assets/81490717/ec92e03d-b6af-4a6b-8e18-d42a7be41182)

![cad2](https://github.com/BurhanNaveed0/Rackify/assets/81490717/c0512520-198d-45a0-8594-70b5868ea8bf)

![IMG_7626](https://github.com/BurhanNaveed0/Rackify/assets/81490717/81264308-35d3-4b13-9a9d-3d455c6e9af8)

## Event Highlights 📸

![DSC_7644-min](https://github.com/BurhanNaveed0/Rackify/assets/81490717/def80458-15e6-4a25-8e8e-b95c818062e5)

![DSC_7452-min](https://github.com/BurhanNaveed0/Rackify/assets/81490717/7fe86e3b-9379-43f5-bee7-2b496c41b2ac)

## Reflection 📝

This was a 24 hour project built during the NJIT IEEE Spring 2024 Hackathon. The aim of the project, going along with the theme of the Hackathon, was to create a working prototype of a system to make life easier in an Urban setting. This had to be acomplished with resources provided by IEEE such as general electronic parts (DC Motors, Stepper Motors, RFID Scanners, Resistors, Transistors, etc.), mircocontrollers (ESP32 and the Arduino), and makerspace tools (3D Printers, Lazer Cutting Machines, etc.)

After one hour of brainstorming as a team, we decided that we would stick to the Hacakthon theme category of Urban improvement. We settled on creating a prototype for a bike racking system that could be distributed throughout any city with users being able to pay for a rack via mobile app or with a pre-paid card. Upon deciding the idea, we split up our crew of 5 into teams working on different sectors of the prototype based on their experience with the group being split into a mechanical, hardware, and software subteams. The mech sub-team was responsible for CADing the locking mechanism, 3D printing the gears, lazer cutting the wood frame, and finally putting together the materials. The electrical subteam was responsible for picking the correct parts to direct power to each subunit of the locking mechanims (motors, power sources, etc.), create schematics for the motor control unit and the RFID scanner, and work with the mech team to assemble all electornics onto the bike lock. Lastly the software subteam was responsible for coding the firmware to control the RFID scanner and the locking mehcanism motors. On top of this they also programmed the webserver hosted on the ESP32 chip aswell as a mobile app in order for users to be able to remotely access the bike rack via their mobile devices. Overall the planning process went pretty smooth and the splitting of the group was really effective in making sure the project was completed within the time window provided. 

The project turned out to be an excellent learning experience for all team members. Team members worked to put their prior Engineering/CS knowledge to the task in their respective areas, working fast in a high stress environment with the deadline approaching within 24 hours. They also moved between subteams, gaining experience not only in their specialty but also in other areas they never tried in (Software subteam helping with CADing, Electrical Subteam helping with writing firmware, etc.) The biggest learing experience however was with networking and marketing our product to the judges. Throughout the day team members connected with other students and IEEE board members, exchanging progress reports on projects and helping each other out during technical difficulties. In the last 10 minutes of the hacking period, the team collaborated to create videos and project descriptions to submit on devpost. After selection for top 10, the team presented infront of qualified judges with only 5 minutes to present the project. The presentation forced us to talk about our project on the fly and work on our confidence despite having very minimal sleep from the night before. 

Despite completing our project within the alloted timeframe and winning 3rd place, it is safe so that production was not seamless. While indivdual sections of the project were completed on time and efficiently, the combination of sections was not. For one, the RFID scanner, despite working correctly in an isolated environment, was not working when attached to the locking mechanism, indicating that the re-assembly of the scanner electronics was done incorrectly. Secondly, the motor which theoretically should have been able to power the ring gear used to engage the lock, was not doing so properly. Lastly, on the software side of things, the HTTP request sent from the app to the bike rack was not always being recieved due to the NJIT network's inbound request restrictions.

The main element powering the hardware side of the project was the ESP32 Microcontroller. This microcontroller was an extremely important asset to our project as it allowed us to power our electronics with its GPIO capabilities aswell as handle HTTP requests through its onboard WiFi capabilities. On the firmware side of things, the C++ Arduino Framework was used with the PlatformIO IDE in order to allow for quick and easy development for the board and easy access to countless pre-made drivers for parts like the RFID scanner and the stepper motor. For the mobile application portion of the project, due to the small amount of time left, a simple HTML mock application was created rather than a full fledged React Native app as it was easy to setup and get running for proof of concept. 
