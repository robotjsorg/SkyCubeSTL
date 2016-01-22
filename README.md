## Screenshot
![Alt Text](https://github.com/jmcmahon443/SkyCubeSTL/blob/master/SkycubeSTL480p.gif)

# SkyCubeSTL
Based on work from one of [FlexMonkey's](http://flexmonkey.blogspot.com/) awesome blog posts: [http://flexmonkey.blogspot.com/2015/07/a-first-look-at-model-ios-sky-cube.html](http://flexmonkey.blogspot.com/2015/07/a-first-look-at-model-ios-sky-cube.html). See [FlexMonkey's GitHub](https://github.com/FlexMonkey) for source code:  [https://github.com/FlexMonkey/SkyCubeTextureDemo](https://github.com/FlexMonkey/SkyCubeTextureDemo).

## 3D in XCode 7, Swift, Model I/O (MetalKit)
There are two distinct methods of adding a 3D STL model to an XCode app. The first method uses XCode itself to convert the STL to a built-in SCN (SceneKit scene node) file. This is great because you can use XCode's GUI to manipulate the model (merge models, translate, rotate, shadows, materials).

The second method retains the STL model's file extension. This is interesting because Model I/O can also export to STL. However you lose out on the ability to manipulate the model via a familiar GUI - but you gain more control and the ability to create apps that rapidly iterate a model in some way. For example, imagine importing an STL model, applying some filter to it, and then exporting it back to the user - just like VSCOcam does for images! You could make a mobile app that lets people play with 3D art on their iPhone!

## My Process
The model from 3D Warehouse: [https://3dwarehouse.sketchup.com/model.html?id=3045229f7869e46f1756ffd6185bba#!topic/3dwh/sCwqS376OUg](https://3dwarehouse.sketchup.com/model.html?id=3045229f7869e46f1756ffd6185bba#!topic/3dwh/sCwqS376OUg).

I used the first process described above, for the sake of time. Specifically, I used SketchUp to break up the file into different systems and to export to a 3DS file. Then in 3ds Max I could import the 3DS file, save it as a MAX file, and finally add any solid material. Then I exported to STL and added it to my XCode project. Finally, I converted each STL into a SCN file and merged them together.
