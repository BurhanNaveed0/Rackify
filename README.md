## Rackify

A prototype bike racking system allowing users to pay to access bikes racks distributed across major cities via mobile app or pre-paid card. 
Achieved 3rd place overall at NJIT’s spring 2024 IEEE Hardware Hackathon, winning a $500 cash prize.

Team Members: Matthew Levine, Prabhav Sharma, Tanush Tammanagoudar, Raghav Bharath

## Project Status
Hackathon project complete. Post competition finishing touches in development:

- Transferring mock HTML mobile app to React Native for demoing on Expo.
- Adding user Authentication with Firebase.
- Handling rack occupation data in Firebase. 

## Project Screen Shot(s)

#### Example:   

[ PRETEND SCREEN SHOT IS HERE ]

[ PRETEND OTHER SCREEN SHOT IS HERE ]


## Reflection

  - What was the context for this project? (ie: was this a side project? was this for Turing? was this for an experiment?)
  - What did you set out to build?
  - Why was this project challenging and therefore a really good learning experience?
  - What were some unexpected obstacles?
  - What tools did you use to implement this project?
      - This might seem obvious because you are IN this codebase, but to all other humans now is the time to talk about why you chose webpack instead of create react app, or D3, or vanilla JS instead of a framework etc. Brag about your choices and justify them here.  

This was a 24 hour project built during the NJIT IEEE Spring 2024 Hackathon. The aim of the project, going along with the theme of the Hackathon, was to create a working prototype of a system to make life easier in an Urban setting. This had to be acomplished with resources provided by IEEE such as general electronic parts (DC Motors, Stepper Motors, RFID Scanners, Resistors, Transistors, etc.), mircocontrollers (ESP32 and the Arduino), and makerspace tools (3D Printers, Lazer Cutting Machines, etc.)

After one hour of brainstorming as a team, we decided that we would stick to the Hacakthon theme category of Urban improvement. We settled on creating a prototype for a bike racking system that could be distributed throughout any city with users being able to pay for a rack via mobile app or with a pre-paid card. Upon deciding the idea, we split up our crew of 5 into teams working on different sectors of the prototype based on their experience with the group being split into a mechanical, hardware, and software subteams. The mech sub-team was responsible for CADing the locking mechanism, 3D printing the gears, lazer cutting the wood frame, and finally putting together the materials. The electrical subteam was responsible for picking the correct parts to direct power to each subunit of the locking mechanims (motors, power sources, etc.), create schematics for the motor control unit and the RFID scanner, and work with the mech team to assemble all electornics onto the bike lock. Lastly the software subteam was responsible for coding the firmware to control the RFID scanner and the locking mehcanism motors. On top of this they also programmed the webserver hosted on the ESP32 chip aswell as a mobile app in order for users to be able to remotely access the bike rack via their mobile devices. Overall the planning process went pretty smooth and the splitting of the group was really effective in making sure the project was completed within the time window provided. 



#### Example:  

This was a 3 week long project built during my third module at Turing School of Software and Design. Project goals included using technologies learned up until this point and familiarizing myself with documentation for new features.  

Originally I wanted to build an application that allowed users to pull data from the Twitter API based on what they were interested in, such as 'most tagged users'. I started this process by using the `create-react-app` boilerplate, then adding `react-router-4.0` and `redux`.  

One of the main challenges I ran into was Authentication. This lead me to spend a few days on a research spike into OAuth, Auth0, and two-factor authentication using Firebase or other third parties. Due to project time constraints, I had to table authentication and focus more on data visualization from parts of the API that weren't restricted to authenticated users.

At the end of the day, the technologies implemented in this project are React, React-Router 4.0, Redux, LoDash, D3, and a significant amount of VanillaJS, JSX, and CSS. I chose to use the `create-react-app` boilerplate to minimize initial setup and invest more time in diving into weird technological rabbit holes. In the next iteration I plan on handrolling a `webpack.config.js` file to more fully understand the build process.
