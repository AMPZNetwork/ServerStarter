# Installing OpenJDK17 on Linux, Windows and MacOS
-----------------------------------

With the release of Minecraft 1.21 significant changes have occurred, necessitating the use of Java 21 to run the game or a server. While the game client now includes a bundled copy of Java 21, it is essential to ensure that Java 21 is installed on your system. To facilitate this process, please refer to the following guide for installing Java 17 on your operating system.

<details>
  <summary>Windows Guide</summary>

# Installing OpenJDK21 on Windows
Before you can start your 1.21x Modded Minecraft server, ensure that Java 21 is installed. Follow the steps below:
1. Begin by downloading the recommended version of OpenJDK17: [v21.0.2](https://aka.ms/download-jdk/microsoft-jdk-21.0.2-windows-x64.msi).
2. Once the download is complete, launch the downloaded `.msi` file and follow the setup instructions provided.
3. Next, return to the server file directory and locate the `forge-1.21-XX.XX.XX-installer.jar` file.
4. Double-click on the `forge-1.21-XX.XX.XX-installer.jar` file to initiate the installation process.
5. After installation, execute the `run.bat` file to start loading the server. Upon the first run, it will pause to prompt your acceptance of the End-User License Agreement (EULA). Locate the EULA in the root directory of your server, provide your consent, and then restart the server for smooth operation.

</details>

<details>
  <summary>Linux Guide</summary>

## Installing OpenJDK on Linux 

For Debian-based Distros (Ubuntu, Pop Os, Linux Mint, etc.), open your terminal and execute the following command:<br>
`sudo apt install openjdk21-jdk -y`

For Arch-based Distros (Manjaro, ArcoLinux, EndeavourOS, etc.), open your terminal and execute the following command:<br>
`sudo pacman -S jre21-openjdk-headless jre21-openjdk jdk21-openjdk openjdk21-doc openjdk21-src`

2. Once you have successfully installed Java 17 on your Linux distribution, you can proceed by running the following command inside the root of your server folder in a terminal:<br>
`bash ./run.sh` 
3. IIf you encounter any issues while running the command, it is likely because the .sh file does not have executable permissions. To resolve this, you can enable the .sh file to be executable by executing the following command:<br>
`chmod +x run.sh`
4. This will grant the necessary permissions to the run.sh file, allowing you to run it without any issues. Please ensure that you have a terminal application available on your system to execute these commands.

</details>

<details>
  <summary>MacOS Guide</summary>

## Installing OpenJDK on macOS
To install OpenJDK on macOS, you can follow these steps:
1. Visit the official [OpenJDK](https://aka.ms/download-jdk/microsoft-jdk-21.0.2-macos-x64.pkg) website in your web browser.
2. Once the download is complete, locate the downloaded "tar.gz" file and open Terminal (located in Applications > Utilities).
3. In Terminal, navigate to the directory where the "tar.gz" file is located. For example, if the file is in the Downloads folder, you can use the following command:<br>
`cd Downloads`
4. Extract the contents of the "tar.gz" file using the following command:<br>
`tar -xvf <filename>.tar.gz`
Replace <filename> with the actual name of the downloaded file.
5. Move the extracted folder to the desired location. For example, you can move it to the /Library/Java/JavaVirtualMachines directory using the following command:
`sudo mv <extracted_folder> /Library/Java/JavaVirtualMachines/` Replace <extracted_folder> with the name of the extracted folder.
6. Set the JAVA_HOME environment variable by opening Terminal and running the following command:<br>
`export JAVA_HOME=/Library/Java/JavaVirtualMachines/<extracted_folder>/Contents/Home`
7. Add the Java bin directory to your PATH variable by running the following command:<br>
`export PATH=$JAVA_HOME/bin:$PATH`
8. Verify the installation by running the following command in Terminal:<br>
`java -version` This should display the version information for OpenJDK 17.

If you are a Mac user and would like to contribute to improving this section, we encourage you to reach out to LabsZero on our Discord. As the guide's author does not personally use MacOS, there is a possibility that the instructions provided may not be perfect for that platform. Your input and expertise would be greatly appreciated in refining the guide for Mac users.

</details>

<details>
  <summary>Common Troubleshooting Fixes</summary>

## Troubleshooting
If you encounter an error in the server console stating:

```
  Caused by: java.lang.module.InvalidModuleDescriptorException: Unsupported major.minor version 60.0
  ```
This indicates that the Java command used in the run script is referencing a different version of Java than the required Java 17. To resolve this issue, follow these steps:

1. Right-click on the run script and open it in a text editor such as NotePad, NotePad++, VisualStudio Code, Sublime, or any other suitable editor. Avoid using a Word editor.

2. Once the file is open, locate the first occurrence of the word "java" in the script.

3. Edit the word "java" to include the full path to your Java 17 installation, enclosed within quotes. The modified line should look similar to this:<br>
`"C:\Program Files\Java\jdk-21.0.2\bin\java" @user_jvm_args.txt @libraries/net/minecraftforge/forge/1.21-XX.X.XX/win_args.txt`

4. By specifying the correct path to Java 21 in the run script, you will resolve the error and ensure that the server runs with the correct Java version

If you need any further support please vist our [Discord](https://discord.ampznetwork.com) and our team will be delighted to assist you..

</details>
-----------------------------------

LASTLY, IF YOU DO NOT WANT TO SETUP THE SERVER YOURSELF WE RECOMMENED BISECT HOSTING:
Approx. $10 - $25 a month depending on what plan you choose. You can also get 25% off with Code AMPZ.

Go to https://www.bisecthosting.com/AMPZ and order a plan which fits you. We suggest at least 6GB per player but nothing lower than 4GB as our packs needs at least 4GB to run.
