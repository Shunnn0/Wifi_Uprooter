## Wi-Fi Uprooter  
This Python script allows you to retrieve Wi-Fi profiles and their passwords on a Windows system using the  "netsh"  command. It provides a convenient way to view Wi-Fi credentials for profiles configured on the machine.

## Prerequisites :
1- Python 3.x

The script will execute and display a list of Wi-Fi profiles and their corresponding passwords, if available.

## How it Works

The script uses the subprocess module in Python to execute Windows command prompt commands (netsh commands) and retrieve the necessary information. Here's a breakdown of the script's workflow:

It executes the command netsh wlan show profiles to retrieve a list of Wi-Fi profiles configured on the system.

For each profile, it executes the command netsh wlan show profile <profile_name> key=clear to obtain detailed information about the profile, including the password.

The script then parses the output to extract the profile names and passwords.

Finally, it prints the profile names and their corresponding passwords in a formatted manner.

Example Output
![w](https://github.com/Shunnn0/Wifi_Uprooter/assets/109821533/aec87d14-3a4d-4ff4-b45a-5e351fe50b20)

In this example, "Network1" and "Network2" are Wi-Fi profiles with their respective passwords displayed. "Network3" does not have a password associated with it.
