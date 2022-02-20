# Rover Instructions

Please follow this comprehensive guide to run the rover. Be prepared mentally to Google errors if any before contacting your seniors :)

# On the frontend laptop:

 1. Start the electron server and click the propulsion button.
 2. Wait for **Backend laptop** to complete step 4.
 3. Join the same network as Jetson.
 4. Change the IP in the propulsion file at 2 spots.
 5. Open a new terminal and run `python3 propulsion.py` . Make sure you are in correct directory before running this.
 6. Give the commands after pressing enter
	 
# On the backend laptop:

 1. Connect the Jetson to your Hotspot.
 2. Check the IP of Jetson using the phone and **ssh into Jetson**. Commands provided in next point.
 3. `ssh ares@<ip of jetson>`
 4. `password: ares1234`
 5. Go to the correct directory `Desktop/Rover-Programs/RoverServer`
 6. Run `python3 server.py`
 7. Check in the terminal whether the data is being received and there's a line saying connection established. 
	 

# Debugging

 1. Open the VNC viewer and enter the ip of Jetson in the top bar.
 2. Use `password: ares1234` to enter the Jetson.
 3. Go to the `Desktop/Rover-Programs/RoverServer` to find the files.
 4. Open the files and use your Debugging skills to find the error.

# Finding right port:

 1. Open Aurdino IDE.
 2. Go to tools.
 3. Open ports. And write down all the given ports on paper and close it.
 4. Go to propulsion folder in the above provided directory. Go to the only file in the folder. And replace the port currently it is "/devtty1".
