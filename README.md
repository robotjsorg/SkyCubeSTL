# SkyCubeSTL
Based on work from this blog post: http://flexmonkey.blogspot.com/2015/07/a-first-look-at-model-ios-sky-cube.html

A test of adding an STL model to SceneKit. Trying to get the MDLSkyCubeTexture to work with the STL model. See [FlexMonkey's](https://github.com/FlexMonkey) original project. https://github.com/FlexMonkey/SkyCubeTextureDemo

There are two distinct methods of adding a 3D STL model to an XCode app. The first method uses XCode itself to convert the STL to a built-in SCN (SceneKit scene node) file. This is great as you can use XCode's GUI to manipulate the model (translate, rotate, shadows, materials). The second method retains the STL model's file extension. This is interesting because Model I/O can also export to STL. So while you lose out on the ability to manipulate the model - you gain more control and the ability to create apps that rapidly iterate a model in some way. Basically, imagine importing an STL, applying a material filter to it, and then export it back to the user - just like VSCOCam for images!
