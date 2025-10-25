# Drone-Delivery-Simulation
 FOCP Assignment 1
 
                  #Task members and role divisions
     NAME                             ROLE                                      
                                   Team leader                                  
    Muhammad Talal Aqdas           Logic and Algorithm Designer
                                   GitHub manager
                                   1st Programmer

                                   2nd programmer
    Maryam Ateeq                   Flowchart Designer
                                   Researcher

                                   Documenter(Word and readme file)  
    Sarim Farooq Khan              Addition of comments
                                   Code and Logic Tester

                                   
                              #Description
  This project simulates a delivery drone that needs to deliver packages to three locations (A, B, and C) in one day.
Before each flight, the drone checks:
   -Weather conditions (Sunny / Windy / Rainy)
   -Battery level
   -Presence of obstacles (like birds or restricted zones)
 
 Based on these, it decides whether to:
   -Deliver successfully,
   -Delay the delivery, or
   -Return to base for recharge.

This is interesting because drones are widely used in modern delivery systems, and this simulation shows how decision-making logic works under random environmental conditions.

                         #Functions used and their explanation

1. getWeather() – Randomly generates weather as “Clear”, “Rainy”, or “Windy”.
2. checkObstacle() – Randomly decides if an obstacle is detected.
3. deliver(location) – Handles all decisions for each delivery (weather, battery, obstacles).
4. summary() – Displays mission summary (successful, delayed, failed deliveries, final battery).

                          # Working

The drone starts with 100% battery.
For each delivery location (A, B, C):
Random weather and obstacles are generated using rand() and srand(time(0)).
-If it’s Rainy → delivery delayed.
-If it’s Windy and battery < 40% then drone recharges (+10%).
-If Obstacle detected then extra 15% battery usage.
-Otherwise, delivery succeeds.
-After all deliveries, a summary is displayed.

Random function rand() are used to create random situations for weather and obstacles each time the program runs.
