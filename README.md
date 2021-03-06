# M1-AirPodOSC

### Description
Initial OSC transmitter for Apple AirPods Pro or any other device supported by [CoreMotion's Headphone Motion Manager](https://developer.apple.com/documentation/coremotion/cmheadphonemotionmanager).

Use this to utilize direct headtracking with [Mach1 Spatial System](https://www.mach1.tech/spatial-system): [M1-Monitor](https://www.mach1.tech/spatial-system#monitor) plugin while mixing (or reviewing) spatial audio content.

For more information about the Mach1 Spatial framework and using it to create your own spatial audio pipeline and content handling please visit the Mach1 Spatial SDK repo: https://github.com/Mach1Studios/m1-sdk

### Setup
 - run `pod install`
 - open .xcworkspace file
 
#### Requirements
 - Xcode 12 Beta Preview 6 or higher (including Xcode 12)
 - iOS 14 or higher

### OSC Orientation Output
Outputs with this Euler angle convention: 

#### [Mach1 Internal Angle Standard](https://dev.mach1.tech/#mach1-internal-angle-standard): Orientation Euler
- Yaw[0]+ = rotate right [Range: 0->360 | -180->180]
- Yaw[0]- = rotate left [Range: 0->360 | -180->180]
- Pitch[1]+ = rotate up [Range: -90->90]
- Pitch[1]- = rotate down [Range: -90->90]
- Roll[2]+ = tilt right [Range: -90->90]
- Roll[2]- = tilt left [Range: -90->90] 

_The orientation convention is based on the first person perspective point of view to make interfacing as easy to interpret as possible._

For more information please read about describing 3D motions here: https://research.mach1.tech/posts/describing-3d-motion

### Notes
 - Ensure to add the required Privacy descriptions in the `Info.plist`

