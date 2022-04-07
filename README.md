# Crossplatform-Multiplayer-Rover-AR-Demo
This is the NASA Perseverance rover in an Augmented Realtiy experience hosted in the web. This was built in Unity with Photon Pun 2 for the mulitplayer neteworking and MRTK for the interactions on various device platforms and WebXR /WebGL to convert the project into a format compatible with the web. 

![RoverWebXRLuminaryGIF](https://user-images.githubusercontent.com/49875750/162324117-86edd156-6d24-4d34-8751-69273b69847a.gif)


Requirements:
- Unity 2019.4.24f1 (Allegedly works up to 2020.3 LTS but I've only been successful with 2019.4LTS)
Any XR enabled device and compatible XR enabled browser
- Quest 1 & 2 (Native browser support)
- PCVR HMD's (Use WebXR API Emulator Browser Plugin) 
- HoloLens 1 & 2 (Native browser support)
- iOS (Safari is not currently an XR enabled browser. Use free 3rd party XR enabled browser: 
Mozilla WebXR Viewer)
- Android (Native browser support)
- PC (Native Browser Support)


**SWXR Sample Setup**
**Option 1 - Clone from original example:**
1) Clone the Simple WebXR Repository from Rufus at https://github.com/Rufus31415/Simple-WebXR-Unity or follow his instructions to build your own version of his project from scratch in his "Quick Start" section of the repositories' readme. 
2) Open or create the project in Unity 2019.4.24 (Documentation indicates this works with newer versions of Unity but I've been unsuccessful) 
3) Switch the build platform to WebGL 
File > Build Settings > Platform > Select WebXR and Switch Platform
4) Set WebGL Template in project settings to "WebXR_Unity2019andBefore"
Edit > Project Settings > Publishing Settings > WebGL Template > Select "WebXR_Unity2019andBefore"
5) Create a WebGL Build of the project
6) Once complete check if your build contains the JavaScript files:
"webxr"
"gl-matrix-min"
7) If you have the above files in your build, you are ready to proceed to the next step, if not, you must follow the steps below. Download my open source Unity package from GitHub containing the two missing JavaScript files listed above. Once downloaded, drag and drop the two JavaScript files into the top file structure of your WebGL project build (with the index file) and you should have everything you need to proceed.
8) Upload your completed build files to a new GitHub repository (index and the above JavaScript files must not be inside of a folder) 
9) Use GitHub pages to host your build in the Web with https enforced security. Also save the GitHub pages link in an easily accessible place like the readme file.
10) Access this GitHub pages web link with any XR enabled device for AR/VR in the web! Supported devices I've tried this with include: 
- HoloLens 2
- Quest 1 & 2
- iOS (Mobile phones and tablets via XR enabled browser)
- Mozilla WebXR Viewer (free XR enabled browser for iOS)
- Android (Mobile phones and tablets)
- WebXR API Emulator on Computers

**Option 2 - Clone from my example:**
1) Download my custom version of the Simple WebXR project which should already have everything you need implemented here:
https://drive.google.com/file/d/1zGKi7He-ZQ6LkWiZwUHp4j0sklwUwqdT/view?usp=sharing
2) Unzip the file and setup the unity project in a location of your choosing. 
3) Open my SWXR (SimpleWebXR) project in Unity 2019.4.24 (Documentation indicates this works with newer versions of Unity but I've been unsuccessful)
4) Switch the build platform to WebGL 
 File > Build Settings > Platform > Select WebXR and Switch Platform
5) Set WebGL Template in project settings to "WebXR_Unity2019andBefore"
 Edit > Project Settings > Publishing Settings > WebGL Template > Select "WebXR_Unity2019andBefore"
6) Create a WebGL Build of the project
 Edit > Build Settings > Select Build
7) Once complete double check if your build contains the JavaScript files (it should in my modified version of SWXR because I created a new WebGL template for WebXR that includes the missing JavaScript files from Rufus's original Simple Web XR sample)
 "webxr"
 "gl-matrix-min"
8) If you have the above files in your build, you are ready to proceed to the next step, if not, you must follow the steps below. Download my open source Unity package from GitHub containing the two missing JavaScript files listed above. Once downloaded, drag and drop the two JavaScript files into the top file structure of your WebGL project build (with the index file) and you should have everything you need to proceed.
9) Upload your completed build files to a new GitHub repository (index and the above JavaScript files must not be inside of a folder) 
10) Use GitHub pages to host your build in the Web with https enforced security. Also save the GitHub pages link in an easily accessible place like the readme file.
11) Access this GitHub pages web link with any XR enabled device for AR/VR in the web! Supported devices I've tried this with include: 
- HoloLens 2
- Quest 1 & 2
- iOS (Mobile phones and tablets via XR enabled browser)
- Mozilla WebXR Viewer (free XR enabled browser for iOS)
- Android (Mobile phones and tablets)
- WebXR API Emulator on Computers

Live Examples
 
MRTK Interaction Examples in WebXR:
- MRTK All Samples in one WebXR Scene: https://calebcram.github.io/WebXR-AllMRTK-Samples/
- MRTK Hand Interaction Sample in WebXR: https://calebcram.github.io/WebXR-MRTK-HandInteraction/
- MRTK Color Picker sample in WebXR: https://calebcram.github.io/Simple-WebXR-ColorPicker/
- MRTK Solver sample in WebXR: https://calebcram.github.io/WebXR-MRTK-Solvers/
- MRTK Dock sample in WebXR: https://calebcram.github.io/WebXR-MRTK-Dock/
- MRTK Elastic System sample in WebXR: https://calebcram.github.io/WebXR-MRTK-Elastic-System/
- MRTK Hand Coach sample in WebXR: https://calebcram.github.io/WebXR-MRTK-Hand-Coach/
- MRTK Hand Menu Layout sample in WebXR: https://calebcram.github.io/WebXR-MRTK-HandMenuLayout/
- MRTK Material Gallery in WebXR: https://calebcram.github.io/WebXR-MRTK-Material-Gallery/
- MRTK Scrolling Object Control samples in WebXR: https://calebcram.github.io/WebXR-MRTK-Scrolling-Objects/

Custom AR/VR Examples in WebXR:
- Spatial Painter Sample in WebXR: https://calebcram.github.io/PainterWebXR_CalebsBuild/
- Interactive VR environment in WebXR: https://calebcram.github.io/AllInReality_WebXRDemo/
- Hand Detection Sample in WebXR: https://calebcram.github.io/WebXR-HandDetection/
- Marker-less WebAR in WebXR: https://calebcram.github.io/MarkerlessWebAR_V2/
- HEMM in WebXR (MRTK Dockable interaction): https://calebcram.github.io/WebXR-HEMM/
- JWST in WebXR (MRTK Dockable Interaction): https://calebcram.github.io/WebXR-JWST/
- Photon MRTK Crossplatform Multiplayer Rover interaction Demo: https://calebcram.github.io/Crossplatform-Multiplayer-Rover-AR-Demo/

![RoverWebXRLuminaryGIF_MultiUser](https://user-images.githubusercontent.com/49875750/162326453-66d04e90-f3a1-490b-ae60-712a253dc112.gif)
 
Contact Caleb Cram for any questions.
- LinkedIn: https://www.linkedin.com/in/caleb-cram-developer
- Portfolio: https://calebcram.dev/
- GitHub: https://github.com/calebcram
- YouTube: https://sidequestvr.com/user/1187860
- SideQuest: https://sidequestvr.com/user/1187860
- Email: caleb.cram@gmail.com
