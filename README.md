# SkyCubeSTL
Based on work from one of [FlexMonkey](http://flexmonkey.blogspot.com/)'s awesome blog posts: [http://flexmonkey.blogspot.com/2015/07/a-first-look-at-model-ios-sky-cube.html](http://flexmonkey.blogspot.com/2015/07/a-first-look-at-model-ios-sky-cube.html). See [FlexMonkey's GitHub](https://github.com/FlexMonkey) for source code:  [https://github.com/FlexMonkey/SkyCubeTextureDemo](https://github.com/FlexMonkey/SkyCubeTextureDemo).

This project is a test of adding an STL model to SceneKit. Trying to get the MDLSkyCubeTexture to work with the STL model. 

![iPadAir1_Screenshot](iPadAir1_Screenshot.png)

There are two distinct methods of adding a 3D STL model to an XCode app. The first method uses XCode itself to convert the STL to a built-in SCN (SceneKit scene node) file. This is great because you can use XCode's GUI to manipulate the model (translate, rotate, shadows, materials). The second method retains the STL model's file extension. This is interesting because Model I/O can also export to STL. However you lose out on the ability to manipulate the model via a familiar GUI - but you gain more control and the ability to create apps that rapidly iterate a model in some way. For example, imagine importing an STL model, applying a material filter to it, and then export it back to the user - just like VSCOCam for images! You could make a mobile app that lets people play with 3D art on their iPhone!
