# Comprehensive Guide: Installing Java 8 on Linux, Windows and MacOS
-----------------------------------

<details>
  <summary>Windows Guide</summary>

# Installing Java 8 64bit on Windows
Before you can start your Modded Minecraft server, ensure that Java 8 is installed. Follow the steps below:
1. Download the recommended version of [Java 8 64bit](https://javadl.oracle.com/webapps/download/AutoDL?BundleId=248242_ce59cff5c23f4e2eaf4e778a117d4c5b).
2. Follow the on-screen instructions provided by the installer. Review the installation settings and make any necessary changes. Typically, the default installation settings work fine for most users.
3. Once the download is complete, locate the downloaded file and double-click on it to open the installer.
4. Navigate back to the server file folder and double-click on the "forge-X.XX.X-XX.XX.XX-installer.jar" file. Please note that the X.XX.XX.XX placeholder should be replaced with the specific version of Forge included in the server files.
5. Once the installer is complete head back to the server folder and Execute the "run.bat" file to initiate the server loading process. However, it will halt the first time, requiring your agreement to the End-User License Agreement (EULA). Provide your consent to the EULA (this can be found in the root of your server) and then restart the server for it to continue running smoothly.

</details>

<details>
  <summary>Linux Guide</summary>

## Installing OpenJDK on Linux 

For Debian-based Distros (Ubuntu, Pop Os, Linux Mint, etc.), open your terminal and execute the following command:<br>
`sudo apt install openjdk8-jdk -y`

For Arch-based Distros (Manjaro, ArcoLinux, EndeavourOS, etc.), open your terminal and execute the following command:<br>
`sudo pacman -S jre8-openjdk-headless jre8-openjdk jdk8-openjdk openjdk8-doc openjdk8-src`

2. Once you have successfully installed Java 17 on your Linux distribution, you can proceed by running the following command inside the root of your server folder in a terminal:<br>
`bash ./run.sh` 
3. If you encounter any issues while running the command, it is likely because the .sh file does not have executable permissions. To resolve this, you can enable the .sh file to be executable by executing the following command:<br>
`chmod +x run.sh`
4. This will grant the necessary permissions to the run.sh file, allowing you to run it without any issues. Please ensure that you have a terminal application available on your system to execute these commands.

</details>

<details>
  <summary>MacOS Guide</summary>

## Installing OpenJDK on macOS
To install OpenJDK on macOS, you can follow these steps:
1. Visit the Oracle website to download the Java Development Kit (JDK) 8 for macOS. You can access the download page at this link: [Java SE Development Kit 8 Downloads](https://www.oracle.com/java/technologies/javase-jdk8-downloads.html).
2. On the download page, accept the license agreement and choose the appropriate JDK 8 version for macOS.
3. Once the download is complete, locate the downloaded file (usually a DMG file) and double-click on it to open the installer.
4. Follow the on-screen instructions provided by the installer. Review the installation settings and make any necessary changes. Typically, the default installation settings work fine for most users.
5. The installer will copy the JDK files to the specified location on your macOS system.
6. After the installation is complete, open Terminal on your macOS system. You can find Terminal in the Applications > Utilities folder.
7. In the Terminal window, type the following command to verify the JDK installation:<br>
`java -version`
8. If Java 8 is successfully installed, the command will display the version information for JDK 8.

If you are a Mac user and would like to contribute to improving this section, we encourage you to reach out to LabsZero on our Discord. As the guide's author does not personally use MacOS, there is a possibility that the instructions provided may not be perfect for that platform. Your input and expertise would be greatly appreciated in refining the guide for Mac users.

</details>

-----------------------------------

LASTLY, IF YOU DO NOT WANT TO SETUP THE SERVER YOURSELF WE RECOMMENED BISECT HOSTING:
Approx. $10 - $25 a month depending on what plan you choose. You can also get 25% off with Code AMPZ.

Go to https://www.bisecthosting.com/AMPZ and order a plan which fits you. We suggest at least 6GB per player but nothing lower than 4GB as our packs needs at least 4GB to run.
