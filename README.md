# UR3-App-Script

The script has been created to speed-up the opening process for [Universal Robots environment](https://github.com/ros-industrial/universal_robot)

The command sequence consider the robot as a simulator and so in adherence the sequence should be modified for real robot start-up.

## Requirements : 
1. Open the terminal, right click on the background of it and select preferences.
2. Follow profiles, then click on the existing profile and in Command Tab choose "Hold terminal open" for "When command exits"
3. Copy the name of the profile (it will be needed in the bash script)
4. After the profile has been copied, open the script ur3_seq.sh and under profile variable pass your profile name

```
profil=YourProfileName
```

## Notice : 
Depending on how your machine performance you may need to change the sleep time which has been declared between each terminal opening.

```
#for example 10 seconds between each command is called
sleep 10s
```
