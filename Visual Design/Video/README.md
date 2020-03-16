# Video
The system-provided video player offers two viewing modes: full-screen (aspect fill) and fit-to-screen (aspect). By default, the system selects a viewing mode based on a video's aspect ratio, and the user can switch modes during playback. For developer guidance, see [AVPlayerViewController](https://developer.apple.com/documentation/avkit/avplayerviewcontroller).

> 시스템에서 제공하는 영상 플레이어는 두 가지 보기 모드를 제공합니다: 전체 화면(aspect fill) 모드와 화면에 맞춘(aspect) 모드입니다. 기본적으로, 비디오의 방향 비율에 따라 보기 모드를 선택하고, 사용자는 재생되는 동안 모드를 변경할 수 있습니다. 자세한 내용은 다음 문서를 확인하세요.



- **Full-screen (aspect-fill) viewing mode.** The video scales to fill the display. Some edge cropping may occur. This is the default viewing mode for wide video (2:1 through 2.40:1). For developer guidance, see [resizeAspectFill](https://developer.apple.com/documentation/avfoundation/avlayervideogravity/1385607-resizeaspectfill).

  > **전체 화면(aspect-fill) 보기 모드.** 화면을 채우기 위해 영상의 크기를 조정합니다. 가장 자리가 잘릴 수 있습니다. 이 모드는 wide 영상(2:1에서 2.40:1)의 기본 보기 모드입니다. 개발자 가이드는 다음 문서를 확인하세요.

  

- **Fit-to-screen (aspect) viewing mode.** The entire video is visible onscreen. Letterboxing or pillarboxing will occur. This is the default viewing mode for standard video (4:3, 16:9, and anything up to 2:1) and ultra-wide video (anything above 2.40:1). For developer guidance, see [resizeAspect](https://developer.apple.com/documentation/avfoundation/avlayervideogravity/1387116-resizeaspect).

  > **화면에 맞춘(aspect) 보기 모드.** 영상의 모든 부분이 화면에 보입니다. Letterboxing(상하에 2개의 검은 띠가 생기는 것)나 pillarboxing(상하좌우로 검은 띠가 생기는 것)가 발생합니다. 이 모드는 일반적인 영상(4:3, 16:9, 2:1까지의 영상)과 ultra-wide 영상(2.40:1을 넘어가는 영상)의 기본 모드입니다. 가이드는 다음 문서를 확인하세요.

  

#### Exmples of Viewing Modes on iPhone XS

<img width="370" alt="43" src="https://user-images.githubusercontent.com/40762111/76736432-2620b380-67aa-11ea-8039-0959e8061e49.png"> <img width="370" alt="169" src="https://user-images.githubusercontent.com/40762111/76736442-2a4cd100-67aa-11ea-92f9-f86f54e9cde4.png">

<img width="370" alt="21" src="https://user-images.githubusercontent.com/40762111/76736450-2caf2b00-67aa-11ea-82f4-f6217717b2aa.png"><img width="370" alt="219" src="https://user-images.githubusercontent.com/40762111/76736456-2f118500-67aa-11ea-93d0-1d88b6cc994a.png">



**Make sure custom video players behave as expected.** The objective is to fill the display by default when playing video content on full-screen devices. However, if filling the display results in too much cropping, the video should be scaled to fit the screen. You should also allow people to switch between full-screen and fit-to-screen viewing based on their individual preferences. For developer guidance, see [AVPlayerLayer](https://developer.apple.com/documentation/avfoundation/avplayerlayer).

> **커스텀 영상 플레이어는 예상 가능할 수 있어야 합니다.** 목적은 전체 화면 기기에서 영상 콘텐츠를 재생할 때, 기본적으로 화면을 채우는 것입니다. 하지만, 화면을 채우면서 너무 많은 부분이 잘리면, 영상을 화면에 맞추어 조정해야 합니다. 또한 사용자의 개개인의 환경에 맞추어 전체 화면 모드와 화면에 맞춘 모드를 변경할 수 있도록 해야 합니다. 자세한 가이드는 다음 문서를 확인하세요.



#### Examples of Padding on iPhone XS

<img width="370" alt="43video" src="https://user-images.githubusercontent.com/40762111/76736470-32a50c00-67aa-11ea-838b-e761367d0873.png"> <img width="370" alt="219video" src="https://user-images.githubusercontent.com/40762111/76736476-35076600-67aa-11ea-8d78-0e45d61111b6.png">



**Always display video content at its original aspect ratio.** When video content uses embedded letterbox or pillarbox padding to conform to a specific aspect ratio, iOS is unable to correctly scale the video based on the user's choice of viewing modes. Padding embedded within the video frame can cause videos to appear smaller in full-screen mode and fit-to-screen mode. It also prevents videos from displaying correctly in edge-to-edge, non-full-screen contexts, like [Picture in Picture](https://developer.apple.com/design/human-interface-guidelines/ios/system-capabilities/multitasking/) mode on iPad.

> **항상 영상 콘텐츠를 원본의 비율로 보여주세요.** 영상 콘텐츠가 특정한 가로 세로 비율을 따르기 위해서 letterbox나 pillarbox를 padding을 사용하는 경우, iOS는 사용자의 보기 모드 선택에 따라 영상을 올바르게 조정할 수 없습니다. 영상 프레임에 들어가 있는 padding은 전체 화면 모드와 화면에 맞춘 모드에서 영상 화면을 더 작아 보이게 할 수 있습니다. 그것은 또한 iPad의 Picture in Picture 모드와 같은 edge-to-edge, 전체 화면이 아닌 contexts에서 영상이 올바르게 보이는 것을 막습니다.

