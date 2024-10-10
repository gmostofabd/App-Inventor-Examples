# 🌟 App-Inventor-Examples 🌟
This repository showcases **example projects** built with **[MIT App Inventor](http://appinventor.mit.edu/)**, covering key concepts like **IoT**, **hardware interfacing**, **GPS tracking**, and **real-time data handling**. These examples are perfect for **beginners** and **educators** seeking to explore mobile app development and **no-code** programming.

<div align="center" style="border: 2px solid #ddd; padding: 20px; border-radius: 10px; background-color: #f9f9f9; width: 60%; margin: auto;">
  <img src="https://github.com/gmostofabd/App-Inventor-Examples/blob/680ba2abb4c1814fb8930964f33fea66f5886f35/assets/images/AppInventor_Banner_5c.png" alt="H-Bridge Circuit Diagram" width="70%" style="border-radius: 8px;">
</div>

**MIT App Inventor** is a great tool to introduce beginners to **Android** app programming. It is an **open-source**, **cloud-based** programming environment which allows you to make your own **mobile apps**n using a **blocks-based programming language**. You access App Inventor using a web browser (Chrome, Firefox, Safari). With these beginner-friendly tutorials, you will learn the basics of programming apps for Android and iOS phones and tablets.

App Inventor platform is developed by the Massachusetts Institute of Technology (MIT). It is composed of a **DESIGNER** section where you visually design your app layout and a **BLOCKS** sections where you include the code to run your app.


---

</br>

## **✨ App Inventor Features**

| 🌟 **Feature**                     | 📋 **Description**                                                                                   |
|-------------------------------------|-------------------------------------------------------------------------------------------------------|
| 🛠️ **_User-Friendly Interface:_**   | Visual learning with **immediate feedback**, allowing for a hands-on experience.                        |
| 📱 **_Creativity & Problem-Solving:_** | Engages users in **creative projects** while fostering **logical thinking** and innovation.             |
| 🌐 **_Real-World Applications:_**   | Develop **practical skills** that create a solid **foundation for future learning** in real-world tasks. |
| 📡 **_Real-time Data Handling:_**   | Build apps with **cloud storage** and live updates for **seamless real-time experiences**.               |

---

</br>

## **✨ You Will Need:**

<div style="display: flex; justify-content: center; width: 100%;">
  <table style="background-color:#e6f7ff; width:80%; border-collapse:collapse; max-width: 100%;">
    <thead>
      <tr>
        <th style="padding: 10px; text-align: left;">🖥️ <strong>Item</strong></th>
        <th style="padding: 10px; text-align: left;">📋 <strong>Description</strong></th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="padding: 10px; background-color:#ffffff;">💻 <strong>A Mac or Windows computer</strong></td>
        <td style="padding: 10px; background-color:#ffffff;">Ensure your system meets the necessary <strong>system requirements</strong>.</td>
      </tr>
      <tr>
        <td style="padding: 10px; background-color:#f9f9f9;">🌐 <strong>A Wi-Fi connection</strong></td>
        <td style="padding: 10px; background-color:#f9f9f9;">Stable <strong>internet connection</strong> is required to download tools and run apps smoothly.</td>
      </tr>
      <tr>
        <td style="padding: 10px; background-color:#ffffff;">📱 <strong>A phone or tablet</strong></td>
        <td style="padding: 10px; background-color:#ffffff;">You will build a <strong>mobile app</strong>, and it's fun to test it <strong>live</strong> on your device while you build (setup required).</td>
      </tr>
    </tbody>
  </table>
</div>

---

</br>

## **🔑 Keywords**

[MIT App Inventor](http://appinventor.mit.edu/), [IoT](https://en.wikipedia.org/wiki/Internet_of_things), [Mobile App](https://en.wikipedia.org/wiki/Mobile_app), [Android App Development](https://en.wikipedia.org/wiki/Mobile_app), [GPS](https://en.wikipedia.org/wiki/Global_Positioning_System), [Sensors](https://en.wikipedia.org/wiki/Sensor), [Bluetooth](https://en.wikipedia.org/wiki/Bluetooth), [Arduino](https://www.arduino.cc/), [IoT Applications](https://en.wikipedia.org/wiki/Internet_of_things), [No-Code](https://en.wikipedia.org/wiki/No-code_development_platform), [STEAM Education](https://en.wikipedia.org/wiki/STEAM), [Educational Tools](https://en.wikipedia.org/wiki/Educational_technology), [Block-Based Coding](https://en.wikipedia.org/wiki/Visual_programming_language), [Cloud Services](https://en.wikipedia.org/wiki/Cloud_computing)



<div align="center" style="border: 2px solid #ddd; padding: 20px; border-radius: 10px; background-color: #f9f9f9; width: 60%; margin: auto;">
  <img src="https://github.com/gmostofabd/App-Inventor-Examples/blob/2906f05d2ecdd52938ff8c44883406cecefe3c24/assets/images/AppInventor_Banner_2a.png" alt="H-Bridge Circuit Diagram" width="80%" style="border-radius: 8px;">
</div>

---

</br>



## 🌟 Let's Make a Simple Game on MIT App Inventor 🌟


1. Open a blank project
Open a blank project. Drag a Canvas element from the Drawing and Animation section. Rename it to “MyCanvas” and set its dimensions to 300x300. Drag a Label element from User Interface. Call it “ScoreLabel” and set its text to “Score: ---”.

Also from User Interface drag a Button and call it “ResetButton”. Make its text “Reset”. From Sensors drag a Clock element so you can control the interval that the mole jumps around the screen. Call it “MoleTimer”, select “Timer Enabled” and set the TimerInterval to 500.


---

</br>


2. Add an ImageSprite
The next thing we need to do is add an ImageSprite from Drawing and Animation to our Canvas. Make sure the image is on the canvas: it will appear nested under MyCanvas in the Components tab. Download the mole image here. The “Enabled” and “Visible” options should be checked, “Width” and “Height” should be “automatic”, and “Speed” should be 0.0.

---

3. Move the mole
Now let’s switch to the “Blocks” screen so we can add some functionality. We’re going to start with a snippet of code to move the mole. In Procedure, select the block with where you can fill the name and has a “do” action. Change the name to “MoveMole”. The “do” section is where we want to put the blocks for this procedure.

Click on Mole and get the “set mole x” block. This locks to a multiplication block from Math. The first factor is the random fraction block, also from Math. This gives a random number between 0 and 1. The first thing we want on the right factor is a subtraction block from Math. The left hand of the subtraction is the “width” block from MyCanvas. The right side is the “width” block from Mole. We’ll repeat this procedure for the y-element of the Mole. In this case, the width should be changed to height.


---


4. Make another Procedure
We’re going to make another Procedure called “UpdateScore”. Before we create the procedure, we need to make a variable for the score. In the Variables tab, we want an “initialize global” block. We want to attach this to a Math number block with the value 0. In this procedure, we want to set the text of ScoreLabel. From Text, we want a “join” block. The top block is a blank Text block where we can fill in “Score”. Underneath, we want “get” from Variables and change the dropdown to “global score”.

---


5. Line it up with the timer
To make the MoveMole procedure happen with the timer, we need the “when MoleTimer Timer do” block from MoleTimer. Then inside that we use the “call MoveMole” block from Procedures.


---

6. Update the score
Now we need the score to update when we tap on the mole. We start with the “when Mole touched x y do” block from Mole. Then we increment the score. First we need the “set” block from Variables and select “global Score” from the dropdown. We attach this to an addition block in Math. We want to add a “get global Score” block from Variables and a number block from Math with the value set at 1. Then we call the UpdateScore and MoveMole procedures.

---

7. Make the button work
Finally we need to implement the functionality of the button. In ResetButton, get the “when ResetButton click do” block. From Variables, get the “set global Score” and connect it to a Math block with value 0. After that we “call UpdateScore” from Procedure.


---

</br>



Advanced Tips and Enhancements
Taking your Mole Mash game to the next level can be both fun and rewarding. Here are some advanced tips and enhancements to make your game even more exciting:

1. Save the Game State

Saving the game state allows players to resume their progress the next time they play. This is particularly useful for tracking high scores or other persistent game data.

How to Do It: Use TinyDB, a database component in MIT App Inventor, to save and retrieve the score.
2. Add Sound Effects and Music

Sound effects and music make the game more immersive and engaging.

How to Do It: Use the Sound component in MIT App Inventor to add sound effects and background music.
3. Create Interactive Elements

Interactive elements make the game more interactive and fun to play.

How to Do It: Add buttons or interactive objects that players can click to perform actions, such as starting a new game, pausing, or accessing a help menu.
4. Implement Power-Ups and Bonuses

Power-ups and bonuses add an extra layer of strategy and excitement to the game.

How to Do It: Create additional ImageSprites for power-ups and use conditional statements to check if the player has collected a power-up and apply its effects.

---

</br>






## **🚀 Table of Contents**
- [Introduction](#introduction)
- [Features](#features)
- [How to Use App Inventor](#how-to-use-app-inventor)
  - [Step 1: Set Up MIT App Inventor](#step-1-set-up-mit-app-inventor)
  - [Step 2: Create a New Project](#step-2-create-a-new-project)
  - [Step 3: Design the User Interface (UI)](#step-3-design-the-user-interface-ui)
  - [Step 4: Add Functionality with Blocks](#step-4-add-functionality-with-blocks)
  - [Step 5: Connect Your Device](#step-5-connect-your-device)
  - [Step 6: Build and Test the App](#step-6-build-and-test-the-app)
- [Project Examples](#project-examples)
- [Tags](#tags)

---

</br>


## **Introduction to App Inventor**

**[MIT App Inventor](http://appinventor.mit.edu/)** is an innovative, drag-and-drop visual programming platform that empowers users to create fully functional **Android apps**. It simplifies app development by utilizing **block-based coding**, making it accessible for individuals without prior programming experience. With App Inventor, you can quickly design apps that interface with real-world hardware like **sensors**, **IoT devices**, and **Bluetooth** components.


App Inventor is an online tool, meaning you can create apps for phones or tablets right in your web browser. This website offers all the support you'll need to design apps:


> **Perfect for**:
> - **Students** and **hobbyists** interested in building apps
> - **Educators** teaching mobile development or IoT
> - Anyone looking to prototype **IoT applications**

---

</br>




## **✨ App Inventor Features**

- 🛠️ **No coding required** – Simplified drag-and-drop interface  
- 📱 **Mobile hardware integration** – Use device **sensors**, **Bluetooth**, **GPS**, etc.  
- 🌐 **IoT-Ready** – Easily connect your app with **Arduino**, **Raspberry Pi**, or other hardware  
- 📡 **Real-time data handling** – Build apps with cloud storage and live updates  
- 🎓 **Educational tool** – Widely used for teaching mobile development and **STEAM** education  

![App Inventor UI Example](https://appinventor.mit.edu/assets/images/ai2-screenshot.png)  
*Design user interfaces quickly using App Inventor's drag-and-drop system.*

---


</br>


##  **History of MIT App Inventor.**
>  -  MIT App Inventor has its roots in the collaborative efforts between Google and the Massachusetts Institute of Technology (MIT), with a goal of democratizing app development and making programming accessible to everyone, especially beginners. The journey of App Inventor has been shaped by several key milestones:

###  Early Development at Google (2009-2011)
>  -  Google Labs first introduced App Inventor in 2009 under the leadership of Hal Abelson, a renowned computer scientist and professor at MIT. Abelson was on sabbatical from MIT and aimed to create a platform that simplified app development, especially for those without a background in coding.
Google App Inventor was launched in 2010 as an experimental tool, part of Google’s effort to provide a visual programming environment for Android app development. The platform was initially available to a limited audience but quickly gained popularity due to its simplicity and effectiveness.

###  Transition to MIT (2011-2012)
>  -  In 2011, Google announced it would no longer maintain App Inventor, but it donated the source code to MIT. Recognizing its educational potential, MIT took over the project and established the MIT Center for Mobile Learning, under its Media Lab, to continue its development.
In 2012, MIT launched the MIT App Inventor 2 platform. It was a more advanced, cloud-based version of the original App Inventor, allowing users to create, save, and share their apps online.

###  Advancements and Growth (2013-present)
>  -  After its release as MIT App Inventor 2, the platform continued to evolve, gaining support for features such as real-time testing, data storage, and connectivity to external devices like sensors, cameras, and other hardware.
App Inventor has become widely used in schools, universities, and educational programs around the world, teaching students the fundamentals of coding, app design, and problem-solving.

By 2017, the platform had over 6 million users from 195 countries and had seen the creation of over 23 million apps. It has become a go-to tool for introducing programming in educational settings, particularly for younger students.

###  Impact on Education
>  -  App Inventor has been pivotal in promoting computational thinking and encouraging more students, including those from traditionally underrepresented groups in technology, to engage in STEM education. It is especially popular in middle and high schools, where it is used to teach students the basics of programming through real-world projects.

###  Present and Future
>  -  Today, App Inventor continues to expand, supporting advanced features like IoT (Internet of Things) development, artificial intelligence (AI) integrations, and cloud services. MIT remains committed to making app development an accessible, creative, and enjoyable process for learners of all ages.


---

</br>


APP INVENTOR CONTROLS
DESIGNER
The first section called Palette includes all the objects and layout options you can choose and drag onto the screen, that is media, buttons, text labels, images, timer, etc.
The central is the Viewer, that is the visual rendering of your phone screen. Close to the screen, you can see the Components window, where you will see all the objects you added to your screen. In the beginning, you will see just “Screen 1”.
The last section on the left, Properties, regards all the options you can choose to change the attributes of the object you have included in your screen. For example, here are the options for changing your Screen1 attributes like background colour, background image, title, alignment.

---

You can download the project here.


</br>


## **🛠️ How to Use App Inventor**

Follow this step-by-step guide to get started with **MIT App Inventor** and begin building your own apps!

### **Step 1: Set Up MIT App Inventor**
1. Visit the official website: [**MIT App Inventor**](http://appinventor.mit.edu/).
2. Click on **Create Apps!** to open the App Inventor development environment.
3. Log in using your **Google account** to access the app creation dashboard.

### **Step 2: Create a New Project**
1. On the main dashboard, click **Start New Project**.
2. Enter a project name, like `MyFirstApp`, and click **OK**.
3. You’ll be taken to the project workspace, where you can design your app.

### **Step 3: Design the User Interface (UI)**
1. **In the Designer tab**, drag and drop components (e.g., buttons, text boxes, images) from the **Palette** on the left into the **Viewer**.
2. Customize each component’s properties (e.g., text, color, size) using the **Properties panel** on the right.

### **Step 4: Add Functionality with Blocks**
1. Switch to the **Blocks** tab to create the logic behind your app.
2. Drag blocks like `When Button1.Click` from the component list and add **logic** or **control blocks** to perform actions such as changing text, displaying notifications, or interacting with hardware.

   ![Blocks Example](https://appinventor.mit.edu/assets/images/blocks.png)  
   *Block-based coding interface*  

### **Step 5: Connect Your Device**
1. **Live Testing**: Test your app on a real device using the **MIT AI2 Companion** app:
   - Download the [**MIT AI2 Companion**](https://play.google.com/store/apps/details?id=edu.mit.appinventor.aicompanion3) from the Play Store.
   - Open the app, and in App Inventor, go to **Connect** → **AI Companion**.
   - Scan the displayed **QR code** or enter the code to sync your device for live testing.

2. **Emulator**: Alternatively, use the built-in emulator by clicking **Connect** → **Emulator**.

### **Step 6: Build and Test the App**
1. To export your app as an installable APK, click **Build** → **App (save .apk to my computer)**.
2. Once the APK is generated, download and install it on any Android device.

> 🎉 **Tip**: You can use **AI-powered cloud services** like **Firebase** for **real-time data** synchronization.

---

</br>


## **🧪 Project Examples**

Explore these real-world projects to see how you can integrate hardware with **App Inventor**:

1. 🚀 **IoT Temperature Monitor**  
   - A project that reads temperature data from a sensor and displays it on an Android app via **Bluetooth**.

2. 🌍 **GPS Location Tracker**  
   - Tracks and displays real-time **GPS data** on a map interface within the app.

3. 🤖 **Bluetooth-Controlled Robot**  
   - Control a simple **robot** using an Android app and **Bluetooth** commands.

![App Inventor IoT Example](https://appinventor.mit.edu/assets/images/iot-ai2-example.png)  
*IoT projects are a great way to learn hardware interfacing using App Inventor.*

---

</br>



## **📚 Tutorial References**

- [Getting Started with MIT App Inventor](https://appinventor.mit.edu/explore/ai2/tutorials/) *A comprehensive guide to help you begin your journey with MIT App Inventor.*

- [Build Your First App](https://appinventor.mit.edu/explore/ai2/tutorials/firstapp/)  *Step-by-step instructions to create your very first mobile application.*

- [MIT App Inventor Documentation](http://appinventor.mit.edu/explore/ai2/docs/)  *Official documentation containing detailed information on all features and functionalities.*

- [Connecting to Bluetooth Devices](https://appinventor.mit.edu/explore/ai2/tutorials/bluetooth/)  *Learn how to establish a Bluetooth connection between your app and hardware devices.*

- [Using the Location Sensor](https://appinventor.mit.edu/explore/ai2/tutorials/location/)  *A guide to using GPS location data within your applications.*

- [Creating a Simple IoT App](https://appinventor.mit.edu/explore/ai2/tutorials/iot/)  *Instructions for building your first Internet of Things (IoT) application.*

- [How to Use the Firebase Database](https://appinventor.mit.edu/explore/ai2/tutorials/firebase/)  *Learn how to integrate Firebase for real-time data storage and retrieval.*

- [App Inventor for Educators](https://appinventor.mit.edu/explore/ai2/educators/)  *Resources and strategies for educators looking to teach app development.*

- [Advanced Features in MIT App Inventor](https://appinventor.mit.edu/explore/ai2/tutorials/advanced/)  *Explore advanced functionalities to enhance your applications.*

---

</br>


## **📌 Tags**

[MIT App Inventor](http://appinventor.mit.edu/), [Mobile App Development](https://en.wikipedia.org/wiki/Mobile_app), [IoT](https://en.wikipedia.org/wiki/Internet_of_things), [Hardware Interfacing](https://en.wikipedia.org/wiki/Embedded_system), [Sensors](https://en.wikipedia.org/wiki/Sensor), [Bluetooth](https://en.wikipedia.org/wiki/Bluetooth), [GPS Tracking](https://en.wikipedia.org/wiki/Global_Positioning_System), [Real-Time Data](https://en.wikipedia.org/wiki/Real-time_computing), [Arduino Integration](https://www.arduino.cc/), [Robotics](https://en.wikipedia.org/wiki/Robotics), [No-Code Development](https://en.wikipedia.org/wiki/No-code_development_platform), [Cloud Integration](https://en.wikipedia.org/wiki/Cloud_computing)


---


</br>



## ⚗️ **Free Examples Gallery**

More App Inventor Tutorials for Beginners

| | | |
|:-------------------------:|:-------------------------:|:-------------------------:|
|<img width="1604" alt="screen shot 2017-08-07 at 12 18 15 pm" src="https://github.com/gmostofabd/App-Inventor-Examples/blob/bc6ce03a1b035361ec5d01bd53047b61538aa0b6/assets/images/AppInventor_ImageContent_Disgner.png">  Designers Interface |  <img width="1604" alt="screen shot 2017-08-07 at 12 18 15 pm" src="https://github.com/gmostofabd/App-Inventor-Examples/blob/bc6ce03a1b035361ec5d01bd53047b61538aa0b6/assets/images/AppInventor_ImageContent_QRcode.png"> App and QR Code | <img width="1604" alt="screen shot 2017-08-07 at 12 18 15 pm" src="https://github.com/gmostofabd/App-Inventor-Examples/blob/bc6ce03a1b035361ec5d01bd53047b61538aa0b6/assets/images/AppInventor_ImageContent_Windows.png?raw=true"> Pallets, View and Properties |
|<img width="1604" alt="screen shot 2017-08-07 at 12 18 15 pm" src="https://github.com/gmostofabd/App-Inventor-Examples/blob/bc6ce03a1b035361ec5d01bd53047b61538aa0b6/assets/images/AppInventor_ImageContent_des2.png?raw=true"> Online Emulator  |  <img width="1604" alt="screen shot 2017-08-07 at 12 18 15 pm" src="https://github.com/gmostofabd/App-Inventor-Examples/blob/bc6ce03a1b035361ec5d01bd53047b61538aa0b6/assets/images/AppInventor_ImageContent_esi1.png?raw=true"> Tutorial image |<img width="1604" alt="screen shot 2017-08-07 at 12 18 15 pm" src="https://github.com/gmostofabd/App-Inventor-Examples/blob/bc6ce03a1b035361ec5d01bd53047b61538aa0b6/assets/images/AppInventor_ImageContent_intwer.png?raw=true"> Starting Screen |
|<img width="1604" alt="screen shot 2017-08-07 at 12 18 15 pm" src="https://github.com/gmostofabd/App-Inventor-Examples/blob/bc6ce03a1b035361ec5d01bd53047b61538aa0b6/assets/images/AppInventor_Banner_6b.png?raw=true"> Tutorial image 1  |  <img width="1604" alt="screen shot 2017-08-07 at 12 18 15 pm" src="https://github.com/gmostofabd/App-Inventor-Examples/blob/bc6ce03a1b035361ec5d01bd53047b61538aa0b6/assets/images/MIT%20App%20Inventor2%20Tutorials_1.jpg?raw=true"> Tutorial image 2 | <img width="1604" alt="screen shot 2017-08-07 at 12 18 15 pm" src="https://github.com/gmostofabd/App-Inventor-Examples/blob/bc6ce03a1b035361ec5d01bd53047b61538aa0b6/assets/images/MIT%20App%20Inventor2%20Tutorials_3.png?raw=true">Tutorial image 3 |


<br/>
<br/>

---

