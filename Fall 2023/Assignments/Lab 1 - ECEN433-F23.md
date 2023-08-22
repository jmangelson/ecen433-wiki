# Lab 1 - Robot Setup and Calibration[^1]

> [!abstract] Purpose
> The <u>**purpose**</u> of this lab is to: 
> 1. Get your duckiebot set up, calibrated, and operational
> 2. Teach you how to use tools such as
> 	- ```dts``` to connect to your robot (or its ROS network) and run code
> 	- ```roslaunch``` to startup the ROS nodes needed for a given project
> 	- ```rqt_graph``` to observe the graph of ROS nodes and their connections to one another
> 3. Demonstrate the complexity of a real robotic system and enable you to explore a little-bit about how the individual components connect and influence one another. 


## Part I - Duckiebot Assembly

1. Start charging your Duckiebattery! You will need it to be fully charged for your first boot and it may take several hours for it to get up to 100%. Plug it in now while you are working on getting everything else setup and ready to go. It will be your responsibility to keep it charged throughout the semester.
 > [!note] Duckiebot Battery Documentation
 > Documentation for the Duckiebot battery can be found here: [https://docs.duckietown.com/daffy/opmanual-duckiebot/preliminaries_hardware/circuits_batteries/index.html](https://docs.duckietown.com/daffy/opmanual-duckiebot/preliminaries_hardware/circuits_batteries/index.html)
 

2. Assemble your Duckiebot using the link below and tips from the slides in class. You will need to demonstrate your assembled Duckiebot to the TAs in class or during office hours. Please do this even if you were given a fully assembled Duckiebot just to make sure there is not any damage.
> [!note] Assembly Instructions
> Assembly instructions for the DB21M can be found here: [https://docs.duckietown.com/daffy/opmanual-duckiebot/assembly/db21m/index.html](https://docs.duckietown.com/daffy/opmanual-duckiebot/assembly/db21m/index.html) ,
> and for the DB21 here: [https://docs.duckietown.com/daffy/opmanual-duckiebot/assembly/db21j/index.html#assembling-duckiebot-db21j](https://docs.duckietown.com/daffy/opmanual-duckiebot/assembly/db21j/index.html#assembling-duckiebot-db21j) .
> 
> 


**It is suggested that you complete this part of the lab by <u>September 15th</u> at the latest.**
## Part II - Duckiebot Setup and Calibration
3. You should have Duckietown Shell set up correctly on the computer you will be using (either your own native Ubuntu laptop or your personal lab machine). If not, refer to HW1. 

4. Set up a Duckietown account on their website, if you haven't already, configure ```dts``` to use it.
> [!note] Duckietown Account Setup
> Instructions for setup can be found here: [https://docs.duckietown.com/daffy/opmanual-duckiebot/setup/setup_account/duckietown_accounts.html](https://docs.duckietown.com/daffy/opmanual-duckiebot/setup/setup_account/duckietown_accounts.html)
> We suggest you just use your github login.

5. If you haven't already, configure dts to also use your dockerhub account
> [!note] Duckietown Shell and Docker Setup
> Instructions for setup can be found here: [https://docs.duckietown.com/daffy/opmanual-duckiebot/setup/setup_account/docker_accounts.html](https://docs.duckietown.com/daffy/opmanual-duckiebot/setup/setup_account/docker_accounts.html)
## Part III - Lane Following and Inspection


[^1]: Initial lab materials were graciously shared by Paul Robinette at UMass-Lowell.
