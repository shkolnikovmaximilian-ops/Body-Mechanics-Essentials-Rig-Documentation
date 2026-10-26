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

If you only want a certain collection hidden, there is a small circle next to the collections that you can click to "solo" them. Only your chosen selection will be shown in the viewport and the rest will be hidden instantly. You ca

n solo out any collection, at any quantity

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/3032bfe2999596c15af8038602cb9b0ade784d0a/Images/SoloLayerGif.gif)

#

### Mesh Visibility Properties

The mesh visibility properties allow you to hide certain parts of the mesh in the viewport. These custom properties are only exposed when the properties bone has been selected (It looks like a square and its above the character's head). This can be exceptionally useful when you need to focus on certain body parts while animating the character. Hiding the mesh parts in the viewport does not hide them in the final render

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/4ea90bf819b59a90b5cffd3c1dc301740cff0f63/Images/VisLayer.gif)

#

### Mesh Color Properties

The mesh color properties allow you to change the color of the entire character to any color you want. Your color choices will be reflected in your final renders

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/463898481448e42c5e6332907aafba30b67be026/Images/ColLayer.gif)

You can also change the color of the Symbol on the character's chest. This will also be reflected in your final renders

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/fe8d58fe678242e03d4c7141430201b7fc51b748/Images/SymColLayer.gif)

And in case you don't want to see the symbol at all, simply hide it by clicking the "Chest Emblem Visibility" box. An open eye means its visible, a closed eye means it isn't. This will also be reflected in your final renders

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/8b3d69ec5e41a2eea8de5891a5a69e81b6bc3c8f/Images/CHesSymColLayer.gif)

#

# RIG CONTROLS

The Body Mechanics Essentials rig controls can be divided into 4 sections. The Torso, Arms, Fingers, and Legs. The documentation will cover almost of the controls/bones in the rig, how they work, and the recommended way to pose/animate them. I only say "almost all of the controls/bones" because I won't be covering bones that are the exact same and on the right side of the body, or just the same in general in terms of functionality. That would be lengthy and boring in my opinion

Off rip, I recommend setting your bone display settings to "In Front" if you haven't already. I positioned some of the bones in the rig to be inside the character, and it will be much easier to see them with "In front" on

By the way the entire rig can be moved using the Root controller. Its a big square surrounding the character's feet, and it's rig layer is named Root

#

### Torso


The main torso controls include the:
- Head Controller
- Neck Controller
- Left and Right Shoulder Controllers
- Hips Controller
- Torso Controller

These can be found in the rig layer titled "Torso"

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/4be237d127f0acb683f4a388741d7a67fc59e6c6/Images/image16.png)

As you move or rotate the controls, the mesh follows and deforms with them

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/fbe2d76781ad83483858c406b4f1f82b530162ac/Images/TorsoCon.gif)

The torso also has some tweaker controls that call allow you to deform the mesh more specifically. The tweaker controls include the:
- Chest FK
- Spine 1 FK
- Spine 2 FK
- Hips FK
- Neck Tweak 1
- Neck Tweak 2
- Chest Tweak
- Spine 1 Tweak
- Spine 2 Tweak
- Hips Tweak

These can be found in the rig layer titled "Torso - Tweak"

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/fb36e3709278ca9be56b00371448cc71b411bdb2/Images/chesttweak.png)

The torso also includes 3 custom properties that are exposed in the UI when clicking any of the torso controls (minus the shoulders). These custom properties are called Head Follow, Neck Follow, and Torso Parent

If Head Follow is set to 1, the head's rotation will follow the chest's rotation. If its set to 0, the head will not follow any rotations

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/9caf3ebe462aa030a62b471323999a16701761c3/Images/headrot.gif)

The Neck Follow is the same as the head's follow properties. 1 is follow, 0 is not

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/a32d8fb4d5d61d0ec126d30e50b19cefc3765025/Images/Neckrot.gif)

The torso parent property lets you decide wether you want the torso to follow the root or not. Locate the torso parent dropdown in the UI to change the parent of the torso

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/51999b47046811c4414a8a2dc155958e2dfffafd/Images/torsoparent.gif)

#

### Arms

The left and right arms are exactly the same. Same controls, same functionality, same everything. Just on opposite sides of the body

The main arm (FK) controls include the:
- Upper arm Controller
- Forearm Controller
- Hand Controller

These can be found in the rig layers titled "Left Arm - FK" and "Right Arm - FK"

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/fd38a89068fe385fb7eea5f17957069342011e53/Images/Armmain.png)

The main arm (IK) controls include the:
- Hand Controller
- Ik Arm pole Controller

These can be found in the rig layers titled "Left Arm - IK" and "Right Arm - IK"

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/08bb17dd567b83216aa0907c47db3455ae963d76/Images/Fkarm.png)

The arms also has some tweaker controls that can allow you to deform the mesh more specifically. The tweaker controls include the:
- Upper arm tweak
- Forearm Tweak
- Hand Tweak
- Hand Tip Tweak

These can be found in the rig layers titled "Left Arm - Tweak" and "Right Arm - Tweak"

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/51d347bed7a3e182f044c5c7b4be1b4cff7a383f/Images/Armtweak.png)

(There are other "controls" in the IK layer, but they are not actually meant for animating. You can try to move them and stuff, but honestly its pointless in my opinion)

The arms have 2 modes. FK mode (Forward Kinematics) and IK mode (Inverse Kinematics). 

When the arm is in FK mode, the arm acts like a downward chain. When you move the upper arm, the rest of the arm follows. When you move the forearm, only the hand follows. You get the point

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/7f9be1ed155084964a86ea5e548f874e0cb6644f/Images/armfkex.gif)

When the arm is in IK mode, the arm transormations are based on the position of the hand in space

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/1253d87cf1b0dbc3ca1d4504476b462e671b5cca/Images/armikex.gif)

You can switch from IK to FK mode in the UI if a part of the arm is selected wether its in IK or FK mode. The switch mechanism slider is called IK - FK (hand.L or hand.R) A value of 1 means FK, a value of 0 means IK

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/3c720a1ba1b4918113aa9947e0a2a554a742a104/Images/ikswitch.gif)

The rig also comes with IK and FK snapping mechanisms. If the arm were in FK mode and you want it to copy the same transforms as the IK arm, hit FK -> IK (hand.l) (or FK -> IK (hand.r) if you are using the right arm) to make the FK arm snap to the position of the IK arm

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/418b58f7eb603930b47a26428eb78431c5e9b0a7/Images/iktofkarm.gif)

If you want the IK arm to snap to the FK arm, hit IK -> FK (hand.l) (.r with the right arm) to do so

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/932856d4b259b98d1513e6b78f5111707f485c7f/Images/fktoikarm.gif)

The FK arm has an FK exclusive property that allows you to change wether it follows the rotations of the body. Select any FK arm control, and find the FK Limb Follow property in the UI. A value of 1 means the arm will not follow any external rotations. A value of 0 means it will

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/80cb8ac5055537f4a8fdb811ddd86d29d8489b15/Images/armrot.gif)

If you dont want the IK arm to stretch the arm when moving the controls very far, select any part of the arm and find the property called IK Stretch. A value of 1 means the mesh will stretch, a value of 0 means the mesh won't stretch

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/2df14b50359558e62b61fa40bdf771e7d3664c3d/Images/ikstretcharm.gif)

The IK arm includes a "pole target". The purpose of this pole target is to change the direction of the bend when moving the IK arm around. You can turn this off by finding the Toggle Pole property in the UI and turning it off

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/1447896bb901f4f90987988570326f86fb79ccab/Images/poletargetonoffarm.gif)

The IK arm can allow you to change it's parent control. The IK arm naturally follows the torso, but you can change what it follows by clicking the dropdown called IK Parent and pick from the list what you want the arm to follow

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/3f6975875b3d6dfabcc7ff15b87102cd0832188d/Images/ikhandparent.gif)

Lastly, you can also change the parent of the IK arm's pole target. The pole target's parent is the shoulder by default. Click the Pole Parent dropdown and pick from the list what you want the pole target to follow

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/bafbf3c32537d98bf9b969b44986f2ad46c2de3b/Images/ikpoleparentswitch.gif)

#

### Fingers

The left and right fingers are exactly the same. Same controls, same functionality, same everything. Just on opposite sides of the body

The main finger (FK) controls include the:
- Thumb 1 Controller
- Thumb 2 Controller
- Thumb 3 Controller
- Index 1 Controller
- Index 2 Controller
- Index 3 Controller
- Middle 1 Controller
- Middle 2 Controller
- Middle 3 Controller
- Ring 1 Controller
- Ring 2 Controller
- Ring 3 Controller
- Pinky 1 Controller
- Pinky 2 Controller
- Pinky 3 Controller
- Palm 1 Controller
- Palm 2 Controller 
- Palm 3 Controller
- Palm 4 Controller
- Palm Controller

These can be found in the rig layers titled "Left Fingers - FK" and "Right Fingers - FK"

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/afd90bbee2657d317ff8583baa77ca5689e7e743/Images/Fkhand.png)

The main arm (IK) controls include the:
- Thumb Controller
- Thumb IK Tip Controller
- Thumb IK pole Controller
- Index Controller
- Index IK Tip Controller
- Index IK pole Controller
- Middle Controller
- Middle IK Tip Controller
- Middle IK pole Controller
- Ring Controller
- Ring IK Tip Controller
- Ring IK pole Controller
- Pinky Controller
- Pinky IK Tip Controller
- Pinky IK pole Controller

These can be found in the rig layers titled "Left Fingers - IK" and "Right Fingers - IK"

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/afd90bbee2657d317ff8583baa77ca5689e7e743/Images/Ikhand.png)

The Fingers also has tweaker controls for each finger on each hand. Those controls include:
- Thumb 1 Tweak
- Thumb 2 Tweak
- Thumb 3 Tweak
- Thumb 3 Tip Tweak
- Index 1 Tweak
- Index 2 Tweak
- Index 3 Tweak
- Index 3 Tip Tweak
- Middle 1 Tweak
- Middle 2 Tweak
- Middle 3 Tweak
- Middle 3 Tip Tweak
- Ring 1 Tweak
- Ring 2 Tweak
- Ring 3 Tweak
- Ring 3 Tip Tweak
- Pinky 1 Tweak
- Pinky 2 Tweak
- Pinky 3 Tweak
- Pinky 3 Tip Tweak

These can be found in the rig layers titled "Left Fingers - Tweak" and "Right Fingers - Tweak"

![alt text](https://github.com/shkolnikovmaximilian-ops/Body-Mechanics-Essentials-Rig-Documentation/blob/afd90bbee2657d317ff8583baa77ca5689e7e743/Images/Handtweak.png)

Just like the arms, you can switch betwen FK and IK modes for each finger. Click any finger and find the IK - FK (finger of choice) slider and choose from there. A value of 1 means FK, 0 means IK

The finger controls on each finger also include the same IK - FK snapping mechanisms, FK limb follow functions, pole parent functions, IK parent functions, and IK stretch functions as the arms (The values for these properties are also the same)

That's because the fingers are techincally mini arms lol. With that being said, I won't explain all of that again for each finger. That would take ages and it would be repetitive. Refer yourself to the arms section for details on all of those properties. All Example GIFs are shown below

#

### Legs

Like the arms and the fingers, the left and right legs are exactly the same. Same controls, same functionality, same everything. Just on opposite sides of the body

The main leg (FK) controls include the:
- Thigh Controller
- Shin Controller
- Foot Controller
- Toes Controller

These can be found in the rig layers titled "Left Leg - FK" and "Right Leg - FK"

The main leg (IK) controls include the:
- Foot Controller
- Toes Controller
- Ik Arm pole Controller
- IK Foot Heel Controller
- IK Foot Spin Controller

These can be found in the rig layers titled "Left Leg - IK" and "Right Leg - IK"

The legs also has some tweaker controls that call allow you to deform the mesh more specifically. The tweaker controls include the:
- Thigh Tweak
- Shin Tweak
- Foot Tweak
- Toes Tweak

These can be found in the rig layers titled "Left Leg - Tweak" and "Right Leg - Tweak"

The legs share the same IK and FK functions as the arm and fingers. All examples GIFS will be provided as per usual. However there are two additional IK and FK properties that are exclusive to the leg that have not been covered in the documentation. These additional properties are the Roll On Toe, and IK -> FK With Roll (either foot) properties

The Roll On Toe property dictates wether the foot rolls on the toes of the foot or not. When the property value is 0, the natural rolling on toes occurs. When the value is 1, the foot roll bypasses the toes entirely

The IK -> FK With Roll (either foot) property is the same as the IK -> FK (either foot) tool, except that it tries to include the roll of the foot when snapping to the FK position

The usual FK and IK functions are shown below
