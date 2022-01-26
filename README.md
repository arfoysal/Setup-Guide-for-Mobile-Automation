# Setup-Guide-for-Mobile-Automation
Its a guide to Setup for Running Mobile Automation test-cases Using Appium on Your Windows Device
# [Notion site Link for Better view](https://arfoysal.notion.site/Setup-for-Running-Mobile-Automation-test-cases-Using-Appium-on-Your-Windows-Device-f256f5b6ac9642d0aef098ac40a2169b)
# [Github Page link](https://arfoysal.github.io/Setup-Guide-for-Mobile-Automation/)

# Setup for Running Mobile Automation test-cases Using Appium on Your Windows Device

Created: January 21, 2022 11:01 PM
Tags: JAVA, Maven, android, appium, eclipse, mobile_automation, selenium, testng

### Java JDK Download, install, set JAVA_HOME and path in environment’s system variable.

<aside>
💡 If you already have this setup for any java version from Java 8 or above → no need to change or do anything in this step. Just checkout!

</aside>

- [ ]  Download and install Java JDK any version you want from java 8 or above
[https://www.oracle.com/java/technologies/downloads/](https://www.oracle.com/java/technologies/downloads/)
- [ ]  Open Environment Variables and click on the new System variable → set 
Variable name: JAVA_HOME 
Variable value: Your Java SDK Location
    
    ![Untitled](Setup%20for%20Running%20Mobile%20Automation%20test-cases%20Usi%206812715ed4b84088bc8efa61036e6ae1/Untitled.png)
    
- [ ]  Select Path system variables then click on Edit → click on new and write 
%JAVA_HOME%\bin
- [ ]  Test successful Java setup → Open CMD and write 
java -version

### Maven zip file Download, extract set  MAVEN_HOME and path in environment’s system variable.

<aside>
💡 If you already have this setup → no need to change or do anything in this step. Just checkout!

</aside>

- [ ]  Download and extract the Maven Binary zip file inside your Java folder(optional) → to keep everything organized
[https://maven.apache.org/download.cgi](https://maven.apache.org/download.cgi)
    
    ![Untitled](Setup%20for%20Running%20Mobile%20Automation%20test-cases%20Usi%206812715ed4b84088bc8efa61036e6ae1/Untitled%201.png)
    
- [ ]  Open Environment Variables and click new System variable → set 
Variable name: MAVEN_HOME 
Variable value: Your Maven directory
    
    ![Untitled](Setup%20for%20Running%20Mobile%20Automation%20test-cases%20Usi%206812715ed4b84088bc8efa61036e6ae1/Untitled%202.png)
    
- [ ]  Select Path system variables then click on Edit → click new and write 
%MAVEN_HOME%\bin
- [ ]  Test successful Maven setup → Open CMD and write 
mvn -version

### Node.js Download, install, & set path in environment’s system variable.

<aside>
💡 If you already have this setup → no need to change or do anything in this step. Just checkout!

</aside>

- [ ]  Download and install Node JS → it will automatically set system environment required path
[https://nodejs.org/en/](https://nodejs.org/en/)
- [ ]  (Optional) Select Path system variables then click on Edit → click on new and write 
C:\Program Files\nodejs\node_modules\npm\bin
- [ ]  Test successful Node JS /npm setup → Open CMD and write 
node -v
npm -v

### Appium Download & install.

- [ ]  Appium server CLI → Open CMD and write 
npm install – g appium           // it will download and install the latest stable release [-g for global install so that you can use it from anywhere]
- Appium server GUI
    - [ ]  Download and install Appium server GUI (optional if already installed in CLI server) 
    [https://github.com/appium/appium-desktop/releases/tag/v1.22.0](https://github.com/appium/appium-desktop/releases/tag/v1.22.0)
    - [ ]  Appium-Inspector Download and install
    [https://github.com/appium/appium-inspector/releases](https://github.com/appium/appium-inspector/releases)
- [ ]  Test successful Appium setup → Open CMD and write 
appium -v

### Android Studio Download, install, set ANDROID_HOME and path in environment’s system variable.

- [ ]  Download and install Android Studio
[https://developer.android.com/studio](https://developer.android.com/studio)
- [ ]  Open Environment Variables and click on the new System variable → set 
Variable name: ANDROID_HOME 
Variable value: Your Android SDK Folder Location
    
    ![Untitled](Setup%20for%20Running%20Mobile%20Automation%20test-cases%20Usi%206812715ed4b84088bc8efa61036e6ae1/Untitled%203.png)
    
- [ ]  Select Path system variables then click on Edit → click on the new and add this four path variables and @important make sure they remain in this order 
%ANDROID_HOME%\emulator
%ANDROID_HOME%\tools
%ANDROID_HOME%\platform-tools
%ANDROID_HOME%\tools\bin
    
    ![Untitled](Setup%20for%20Running%20Mobile%20Automation%20test-cases%20Usi%206812715ed4b84088bc8efa61036e6ae1/Untitled%204.png)
    

### Android Studio SDK Manager Setup

- [ ]  Open Android SDK manager from the Tool tab
- [ ]  Select SDK Platforms →
Checked & installed “Android API 32” and at least one Android version
    
    ![Untitled](Setup%20for%20Running%20Mobile%20Automation%20test-cases%20Usi%206812715ed4b84088bc8efa61036e6ae1/Untitled%205.png)
    
- [ ]  Select SDK Tools → Uncheck Hide Obsolete Packages ⇒ Checked & installed
1. Android SDK Build-tools 32
2. Android Emulator
3. Android SDK Platform-Tools
4. Android SDK Platform-Tools(Obsolete)
5. Intel x86 Emulator Accelerator (HAXM installer)
    
    ![image_2022-01-23_132029.png](Setup%20for%20Running%20Mobile%20Automation%20test-cases%20Usi%206812715ed4b84088bc8efa61036e6ae1/image_2022-01-23_132029.png)
    
- [ ]  Select SDK Update site → make sure all listed items are Enabled

### Android Studio AVD(Android Virtual Devices) Manager Setup / Emulator

- [ ]  Open Android AVD Manager from the Tool tab
- [ ]  Click on click Create Virtual Device ⇒ <Choose a device definition / a model > ⇒ Next ⇒ <Select system Image/ android version> ⇒ Next → provide ADV/emulator name > Finish
- [ ]  Done! you just create Android Virtual Device
- [ ]  From the Actions column, you can perform Launch, Edit, Duplicate, Wipe data,  Cold boot now, Delete .etc on your selected AVD device.

### Physical Device setup

- [ ]  Go To Your phone Settings and Tap About Phone option
- [ ]  keep Tapping on Your device version option → Until the bottom popup shows 
“No Need, You are already a developer”
- [ ]  Now search within your settings by typing “Developer options” and Tap on it.
- [ ]  Now make sure the below three options are enabled
    1. USB debugging
    2. Install via USB
    3. USB debugging (Security Settings)
    
    ![Untitled](Setup%20for%20Running%20Mobile%20Automation%20test-cases%20Usi%206812715ed4b84088bc8efa61036e6ae1/Untitled%206.png)
    

### Eclipse or any other IDE download and install

<aside>
💡 If you already have an installed IDE → no need to change or do anything in this step. Just checkout!

</aside>

- [ ]  Download and install Eclipse IDE
[https://www.eclipse.org/downloads/](https://www.eclipse.org/downloads/)
- [ ]  (Optional) Add multiple Java JDK in your Eclipse {if you want}
Install your Java JDK version in any location. [for an organized way keep it inside java folder]
    
    ![Untitled](Setup%20for%20Running%20Mobile%20Automation%20test-cases%20Usi%206812715ed4b84088bc8efa61036e6ae1/Untitled%207.png)
    
    Open Eclipse → Window → Preferences → Java → Installed JREs → Add → Standard VM → Next → JRE home - Directory → select your new JDK home Folder → Finish → Apply 
    
    ![Untitled](Setup%20for%20Running%20Mobile%20Automation%20test-cases%20Usi%206812715ed4b84088bc8efa61036e6ae1/Untitled%208.png)
    
    <aside>
    💡 Done but if Eclipse through an exception on your next open - “Incompatible JVM. Version 1.8.0_261 of the JVM is not suitable for this product. Version: 11 or greater is required”
    
    </aside>
    
    ```bash
    → Open eclipse installed directory and open “eclipse.ini” with text-editor and 
     Past your default javaw.exe location before -vmargs like this way 
    
    -vm
    C:\Program Files\Java\jdk-16.0.2\bin\javaw.exe
    -vmargs
    ```
    

### RUN!

<aside>
💡 To perform the below command without any exception. Please recheck the order of your system path variables for Android. [which we did in the earlier Android Studio section]
”Open CMD from any location and run the below command →whenever you need them”

</aside>

### **Android Debug Bridge(adb)** → udid | install |PackageName |appActivity

### T**o show connected/active adb devices with their Unique Device Identifier(udid)**

```bash
**adb devices**
```

### Install APK ⇒ Many ways! you can do that

→ Drag and Drop the apk file inside the emulator
→ Install using play store 
→ Download apk file using emulator browser than install
→ transfer apk file to emulator storage location than install
→ Install using cmd by the helping of adb(**Android Debug Bridge**)

```bash
# if only one adb device connected to your computer 
adb install "path to .apk"
# if multiple device are connected 
adb -s "device-udid" install "path to .apk"  #-s source/serialNumber/Identifier
# optional options are 
# adb install [options] path -!
#-r: Reinstall an existing app, keeping its data.
#-f: Install package on the internal system memory.
#-d: Allow version code downgrade.
#-g: Grant all permissions listed in the app manifest."
# https://developer.android.com/studio/command-line/adb
```

### packageName and appActivity for any installed App

- Get packageName and appActivityackage using adb shell
    
    Open app in your emulator or physical device and run this command in cmd
    
    ```bash
    # if only one adb device connected to your computer 
    adb shell dumpsys window | find "mCurrentFocus"
    # if multiple device are connected 
    adb -s "device-udid" shell dumpsys window | find "mCurrentFocus"   
    #-s source/serialNumber/Identifier
    ```
    
    ![Untitled](Setup%20for%20Running%20Mobile%20Automation%20test-cases%20Usi%206812715ed4b84088bc8efa61036e6ae1/Untitled%209.png)
    
- Get packageName and appActivityackage using Apk info app
    
    [https://play.google.com/store/apps/details?id=com.wt.apkinfo&hl=en&gl=US](https://play.google.com/store/apps/details?id=com.wt.apkinfo&hl=en&gl=US)
    

### Emulator → List | Launch | Shutdown | Cold boot | Wipe data

- To show List of available emulator names
    
    ```bash
    emulator -list-avds
    ```
    
- Launch/start/Open an Emulator → after start emulator it will keep alive until close this current CMD window.
    
    ```bash
    emulator -avd emulator_Name
    # OR
    emulator @emulator_Name
    ```
    
- Close/Shutdown an Emulator → Many ways are available
    
    → In CMD window simply click Ctrl + C and wait for few seconds →  it will close the emulator.
    
    → By clicking close button in emulator UI
    → Closing the CMD window 
    
- Start Emulator in Cold Boot view
    
    ```bash
    emulator -avd emulator_Name -no-snapshot-load
    # OR
    emulator @emulator_Name -no-snapshot-load
    ```
    
- Wipe-data/RESET an Emulator
    
    ```bash
    emulator -avd emulator_Name -wipe-data
    # OR
    emulator @emulator_Name -wipe-data
    ```
    

### Appium Server

- Appium Server in the CLI
    
    simply type appium in CMD.  it will start the server and keep running until closing the CMD window or→ in CMD window type Ctrl + C for closing the server.
    
    ```bash
    appium
    ```
    
- Appium Server in the GUI
    
    Open Appium server GUI application and click on start button ⇒ run server
    
    For closing the server simply click on close button 
    

### uiautomatorviewer - it's a simple UI inspector. work by taking screenshots

<aside>
💡 Run Appium server and connect a physical device or run emulator first then proceed

</aside>

- Run UI Automator
    
    Simply type uiautomatorviewer in CMD. it will run the UI Automator and keep running until closing the CMD window or→ in CMD window type Ctrl + C for closing the UI Automator.
    
    ```bash
    uiautomatorviewer
    ```
    
- (Optional) if exception present when trying to run UI Automator for the fist time
    
    <aside>
    💡 if there is an exception like this 
    -Djava.ext.dirs=..\lib\x86_64;..\lib is not supported.  Use -classpath instead.
    Error: Could not create the Java Virtual Machine.
    Error: A fatal exception has occurred. Program will exit.
    
    </aside>
    
    steps 1: Download and install java 8 .. [just simple install no need to change anything]
    
    steps 2: open uiautomatorviewer.bat with a text editor from the below location 
                 C:\Users\your_user_name\AppData\Local\Android\Sdk\tools\bin 
    
    step 3: Find these lines of code inside the file
    
    ```bash
    rem Check we have a valid Java.exe in the path.
    set java_exe=
    call ..\lib\find_java.bat
    ```
    
    step 4: Replace with these lines of code and save the file 
    
    ```bash
    rem Check we have a valid Java.exe in the path.
    set java_exe=C:\Program Files\Java\jdk1.8.0_321\jre\bin\java.exe
    rem call ..\lib\find_java.bat
    ```
    
    step 5: Done! now try to run uiautomatorviewer.bat hopefully it will works
    

### Appium inspector - it's an advanced UI inspector for mobile OS

<aside>
💡 Run Appium server and connect a physical device or run emulator first then proceed

</aside>

- Run Appium Inspector
    
    Run Appium Inspector by clicking on and set Remote Path →   /wd/hub
    
- Desired Capabilities
    - To start a session → with an only connected or running adb device
    if multiple devices are connected then it will start with priority one.
        
        ```bash
        {
          "platformName": "android"
        }
        ```
        
    - To start a session with a specific physical or emulator device
        
        ```bash
        {
          "platformName": "android",
        	"udid" : "Your device or emolator udid"
        }
        ```
        
    - To start a session with a specific physical or emulator device and a specific app
        
        ```bash
        {
          "appium:deviceName": "Iblish",
          "platformName": "android",
          "appPackage": "Your app package name",
          "appActivity": "Your app Activity name"
        }
        ```
        
    - To start a session with a specific device & app, and specific automation engine
        
        ```bash
        {
          "appium:deviceName": "Iblish",
          "platformName": "android",
        	"automationName": "UiAutomator2",
          "appPackage": "Your app package name",
          "appActivity": "Your app Activity name"
        }
        ```
        
    - For more Appium Desired Capabilities
        
        [https://appium.io/docs/en/writing-running-appium/caps/](https://appium.io/docs/en/writing-running-appium/caps/)
        

### Eclipse Project → Create | pom.xml | Edit Script |  run a script

- Create a maven project
    
    
- Edit pom.xml
    
    <aside>
    💡 if you are planning to use selenium page factory in your mobile automation  project then use selenium version below 4 to avoid exception → java.lang.NoClassDefFoundError
    
    </aside>
    
    ```xml
    <project xmlns="http://maven.apache.org/POM/4.0.0"
    	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    	xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    	<modelVersion>4.0.0</modelVersion>
    
    	<groupId>arfoysal.com</groupId>
    	<artifactId>mobileautomation</artifactId>
    	<version>0.0.1-SNAPSHOT</version>
    	<packaging>jar</packaging>
    
    	<name>mobileautomation</name>
    	<url>http://maven.apache.org</url>
    
    	<properties>
    		<project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
    	</properties>
    
    	<dependencies>
    
    		<!-- https://mvnrepository.com/artifact/org.testng/testng -->
    		<dependency>
    			<groupId>org.testng</groupId>
    			<artifactId>testng</artifactId>
    			<version>7.5</version>
    			<!--<scope>test</scope> -->
    		</dependency>
    
    		<!-- https://mvnrepository.com/artifact/io.appium/java-client -->
    		<dependency>
    			<groupId>io.appium</groupId>
    			<artifactId>java-client</artifactId>
    			<version>7.6.0</version>
    		</dependency>
    
    		<!-- https://mvnrepository.com/artifact/org.seleniumhq.selenium/selenium-java -->
    		<dependency>
    			<groupId>org.seleniumhq.selenium</groupId>
    			<artifactId>selenium-java</artifactId>
    			<version>3.141.59</version>
    <!-- use below 4 version, if you use upper one you will recevie error start with-java.lang.NoClassDefFoundError:-->
    		</dependency>
    		
    		
    		<!-- https://mvnrepository.com/artifact/org.apache.commons/commons-lang3 -->
    		<dependency>
    			<groupId>org.apache.commons</groupId>
    			<artifactId>commons-lang3</artifactId>
    			<version>3.12.0</version>
    		</dependency>
    
    		<!-- https://mvnrepository.com/artifact/commons-io/commons-io -->
    		<dependency>
    			<groupId>commons-io</groupId>
    			<artifactId>commons-io</artifactId>
    			<version>2.11.0</version>
    		</dependency>
    
    		<!-- https://mvnrepository.com/artifact/commons-validator/commons-validator -->
    		<dependency>
    			<groupId>commons-validator</groupId>
    			<artifactId>commons-validator</artifactId>
    			<version>1.7</version>
    		</dependency>
    		
    	</dependencies>
    </project>
    ```
    
- Edit test script
- Run test script