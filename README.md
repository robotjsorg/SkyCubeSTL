# SkyCubeSTL

A test of adding an STL model to SceneKit. Trying to get the MDLSkyCubeTexture to work with the STL model. See [FlexMonkey's](https://github.com/FlexMonkey) original project below. https://github.com/FlexMonkey/SkyCubeTextureDemo

I've added an STL file with this code:
```
let bundle = NSBundle.mainBundle()
let path = bundle.pathForResource("BUILDINGMETHOD2", ofType: "STL")
let url = NSURL(fileURLWithPath: path!)
let asset = MDLAsset(URL: url)
let sceneKitScene = SCNScene(MDLAsset: asset)

sceneKitScene.rootNode.childNodeWithName("BUILDINGMETHOD2", recursively: false)?.geometry?.materials = [material]
```

# SkyCubeTextureDemo

A demonstration of using MDLSkyCubeTexture in a SceneKit project.

Companion project to this blog post: http://flexmonkey.blogspot.com/2015/07/a-first-look-at-model-ios-sky-cube.html

![Demo gif](/SkyCubeDemonstration/skycube.gif)
