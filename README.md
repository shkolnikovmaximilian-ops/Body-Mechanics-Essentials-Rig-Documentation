# Body Mechanics Essentials Rig Documentation

This README includes common issue fixes, instructions, and guides for how all the controls and custom properties work

As time passes, updates will come to the rig and the README if they are needed

Please feel free to contact me about any issues you face for the rig, or any criticisms/feedback you would like to give. If it's in my power to fix any listed problems, I will fix them

CONTACTS: [EMAIL - shkolnikovmaximilian@gmail.com]


# 

# COMMON ISSUES

### Script Security Error

The only common issue I have found across multiple computers is that when you open the file, this error pops up. This error pops up because the rig automatically comes with a script that runs the rig's custom UI (User Interface). The computer does not recognize the script, and therefore does not trust it

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image.png)

To fix this, either click "Allow Execution" (which will only run the script this one time, meaning you will probably have to click that every time you open the file), or you can check "Permanently enable execution of scripts" so that way the script runs automatically

# 

# HOW TO USE THE RIG IN OTHER BLENDER FILES

When you open a new file and you want to import the rig into it, you can either "Append" or "Link" the rig into it

APPENDING A FILE \- Copies basically all of the file data from the origin file onto your new file. You can freely edit any of this copied data without changing the origin file

LINKING A FILE \- Copies only your selected parts of a file onto your new file, while leaving the unnecessary stuff behind. Any changes you make in the file where this rig came from, will reflect in the new file when you link the rig

#

### Appending the rig (Not Recommended)

1. In your new file click file \>\> Append...

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-1.png)

2. Locate the rig file on your computer, and double click it

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-2.png)

3. Locate the Collection folder and open it

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-3.png)

4. Inside the Collection Folder, locate the "MASTER\_CubeMan\_Enhanced" folder and open it

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-4.png)

5. Your rig will now be available in the scene\! But it's quite a mess... All of the extra data that was used to create the rig is now in this file

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-5.png)

6. To clean all this up, select everything in the outliner outside of the master collection that begins with the prefix WGT

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-6.png)

7. When all of that is selected, right click, and hit "Unlink"

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-7.png)

   Your scene and rig is all cleaned up now! But that was more of a hassle than it needed to be. Let me show you a better way to put the rig in a new file

#

### Linking the rig (Recommended)

1. In your new file click file \>\> Link...

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-8.png)

2. Locate the rig file on your computer, and double click it

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-2.png)

3. Locate the Collection folder and open it

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-3.png)

4. Inside the Collection Folder, locate the "MASTER\_CubeMan\_Enhanced" folder and open it

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-4.png)

5. Your rig will now be available in the scene\! But you are locked out from entering pose mode to start animating the rig. Lets fix that

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-9.png)

6. Right click the Master Collection. Library Override >> Make >> Click Selected & Content

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-10.png)

   Enter Pose Mode and now your rig is ready for animating! This is a much cleaner and effienct way of re-using the rig in other blender files rather than appending it

#

### "Help! I did all of that and the rig's UI is not there! What do I do?!"

It happens sometimes. I honestly don't know why it happens, but I know how to make it appear. You are going to have to run the rig's script manually. If the rig UI is in fact there after following the steps above, then don't worry about this part

#

1. Inside your new file with your rig, enter the Scripting window

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-11.png)

2. Inside the scripting window, locate the little notebook icon and click it. You should see a dropdown menu including a script option with a chain icon, as well as the name of the file you are linking or appending the rig from

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-12.png)

3. Click that script option. For reference, this is what it looks like once opened in the script editor

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-13.png)

4. All you have to do now, is run the script by clicking this little play button up at the top!

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-14.png)

   Go back to the Layout window, and your rig UI will be available!

   ![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9feec754ecb86ed577b2a3f04afe42d26c73ab30/Images/image-15.png)

#

# NAVIGATING THE RIG USER INTERFACE

### Rig Layers

The rig UI is generated using a script that is run when the rig is opened. A crucial component of this UI is the rig layers. The rig layers allow you to hide any bone (control) collection listed in the UI. When a collection is highlighted blue, the collection is visible in the viewport. When the collection is not higlighted blue, the collection is hidden
   
![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/20b7f48ab1a19fb2995bde86db6a234db370fbf5/Images/RigLayersGif.gif)

If you only want a certain collection hidden, there is a small circle next to the collections that you can click to "solo" them. Only your chosen selection will be shown in the viewport and the rest will be hidden instantly. You can solo out any collection, at any quantity

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/3032bfe2999596c15af8038602cb9b0ade784d0a/Images/SoloLayerGif.gif)

#

### Mesh Visibility Properties

The mesh visibility properties allow you to hide certain parts of the mesh in the viewport. This can be exceptionally useful when you need to focus on certain body parts while animating the character. Hiding the mesh parts in the viewport does not hide them in the final render

![alt text]

