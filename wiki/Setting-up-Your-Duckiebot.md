# Setting up your Duckiebot

On this page you will learn how to set up your computer to support the duckietown commands, and how to build the physical duckiebot. One of the steps in the computer setup will be flashing the SD card for your duckiebot. This can easily take over an hour so it is recommended to start that process first, then begin the physical duckiebot assembly to save time.

## Computer Config

### Install dependencies

Install the required dependencies by putting the following lines into the terminal

`sudo apt update`
`sudo apt install -y python3-pip git git-lfs curl wget`

### Install Docker

Docker is a platform that allows us to manage and deploy software applications inside of "containers". We be using it for the Duckietown system. 

Follow the instructions to install docker provided by Duckietown [here](https://docs.duckietown.com/daffy/opmanual-duckiebot/setup/setup_laptop/setup_docker.html)

You will also need to make a docker account by following the instructions [here](https://docs.duckietown.com/daffy/opmanual-duckiebot/setup/setup_account/docker_accounts.html)

### Install the Duckietown Shell

Duckietown Shell (DTS) is a command-line interface that has all of the needed Duckietown operations. To install DTS, use the command:

`pip3 install --no-cache-dir --user --upgrade duckietown-shell`

Confirm the installation by running the test

`which dts`

### Account Setup

First, make sure that you have a github account.

Next, you will need to set the Duckietown software distro. We will be using daffy for this class. Set the shell to the daffy distro with this command

`dts --set-version daffy`

Now you will need to get a Duckietown token. You can get a token by making an account on the Duckietown [website](https://hub.duckietown.com/signin/?next=/profile/).

The token can be found [here](https://hub.duckietown.com/profile/) after creating your account.

Next use the following command then paste your token into the terminal

`dts tok set`

Check your token status by running

`dts tok status`

The Duckietown shell will recognize you as a user if everything is correct.

### SD Card

Once you have the duckietown shell set up, you can now configure the SD card for your duckiebot. Insert the micro-SD into the USB adapter and enter the following command

`dts init_sd_card --hostname HOSTNAME --type duckiebot --configuration DB21J --wifi WIFI`

HOSTNAME = the name of the robot to flash the SD for
WIFI = comma seperated list of wifi networks to connect to. Ex: wife_name1:password,wife_name2:password
    * There shouldnt be any space after the commas

Run the command and follow the instructions in the Duckietown Shell to select the device you want to configure. The shell will then write to the SD card

### Booting the Duckiebot

After powering on the Duckiebot with the SD card inside, the lights will turn on. Allow 10-15 minutes for the boot process to complete. You can check the Duckiebot boot status by running the command:

`dts fleet discover`

This will show the status of all the different duckiebots on the network.

After the Duckiebot has rebooted a few times and the status column reads "Ready", you can now access your Duckiebot's dashboard.

Open your browser and got to http://HOSTNAME.local/. This will bring you to the dashboard of your car

### Powering off the Duckiebot

Duckiebots can be powered down with the following command

`dts duckiebot shutdown HOSTNAME`

Duckiebots can also be rebooted with

`dts duckiebot reboot HOSTNAME`


