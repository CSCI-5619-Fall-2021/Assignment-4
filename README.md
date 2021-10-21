# Assignment 4: Selection and Manipulation

**Due: Thursday, November 4, 10:00pm CDT**

In this assignment, you will implement some more advanced selection and manipulation techniques that were discussed in class.

## Submission Information

You should fill out this information before submitting your assignment.  Make sure to document the name and source of any third party assets such as 3D models, textures, or any other content used that was not solely written by you.  Include sufficient detail for the instructor or TA to easily find them, such as a download link.

Name: 

UMN Email:

Third Party Assets:

## Getting Started

Clone the assignment using GitHub Classroom.  The project has been configured for the Oculus Quest, and the [XR Interaction Toolkit](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@1.0/manual/index.html) package has already been imported.  The project contains more sophisticated versions of the grabbing and pointing scripts we implemented in [Lecture 13](https://github.com/CSCI-5619-Fall-2021/Lecture-13).  Both controllers have the `GraspGrabber` and `PointGrabber` components, both of which extend from the `Grabber` base class.  Every object in the scene is `Grabbable` except for the ground.

## Rubric

Graded out of 20 points. 

1. Implement the **Go-Go** grasping technique (see [Lecture 12](https://www.beautiful.ai/player/-Mm-BRr29z-cOImVB72w), slide 26) on both controllers.  This will involve computing the distance between each controller and the headset.  For distances less than some threshold *d*, the location of the controller should match the user's hand to allow them to easily grab nearby objects.  For distances greater than *d*, the hand should be scaled forward to extend the user's reach.  You should experiment with different values for *d* and the distance scale factor to settings that work comfortably. (6)
   *Hint: you should modify the `localPosition` transform of the `controller_l` and `controller_r` game objects, which are children of the `LeftHand Controller` and `RightHand Controller` game objects, respectively.*
2. The user should be able to toggle the Go-Go- technique on and off using the A button on the right controller and the X button on the left controller. (4)

Make sure to document all third party assets in your readme file. ***Be aware that points will be deducted for using third party assets that are not properly documented.***

## Submission

You will need to check out and submit the project through GitHub classroom.  **Make sure your APK file is in the root folder.** Do not remove the `.gitignore` or `README.md` files.

Please test that your submission meets these requirements.  For example, after you check in your final version of the assignment to GitHub, check it out again to a new directory and make sure everything opens and runs correctly.  You can also test your APK file by installing it manually using [SideQuest](https://sidequestvr.com/).

## Acknowledgments

The scene uses assets from the [Playground Low Poly](https://assetstore.unity.com/packages/3d/environments/playground-low-poly-191533) package from the Unity Asset Store.

## License

Material for [CSCI 5619 Fall 2021](https://canvas.umn.edu/courses/268490) by [Evan Suma Rosenberg](https://illusioneering.umn.edu/) is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).

The intent of choosing CC BY-NC-SA 4.0 is to allow individuals and instructors at non-profit entities to use this content.  This includes not-for-profit schools (K-12 and post-secondary). For-profit entities (or people creating courses for those sites) may not use this content without permission (this includes, but is not limited to, for-profit schools and universities and commercial education sites such as Coursera, Udacity, LinkedIn Learning, and other similar sites).   