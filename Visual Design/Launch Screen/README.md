# Launch Screen
A launch screen appears instantly when your app starts up and is quickly replaced with the app's first screen, giving the impression that your app is fast and responsive. The launch screen isn’t an opportunity for artistic expression. It’s solely intended to enhance the perception of your app as quick to launch and immediately ready for use. Every app must supply a launch screen.

> Launch screen은 앱이 빠르고 즉각 반응하는 인상을 주면서 앱을 시작할 때 즉시 보이고, 빠르게 첫 화면으로 대체됩니다. Launch screen은 미적인 인상을 주기 위한 것이 아닙니다. 단지, 앱이 빠르게 시작하고 즉시 사용할 준비가 되어 있다는 인식을 향상시키기 위한 것입니다.



<img width="561" alt="스크린샷 2020-02-27 오전 9 29 23" src="https://user-images.githubusercontent.com/40762111/75400847-c28e2d80-5943-11ea-90d4-9905897a1d9d.png">

To accommodate the screen sizes of different devices and environments, such as multitasking, use an Xcode storyboard to provide a launch screen. Storyboards are flexible and adaptable, and you can use a single storyboard to manage all of your launch screens. For developer guidance, see [Responding to the Launch of Your App](https://developer.apple.com/documentation/uikit/app_and_environment/responding_to_the_launch_of_your_app).

> 멀티태스킹과 같이 각기 다른 기기의 화면 크기와 환경에 대응하기 위해서, launch screen을 제공하는 Xcode storyboard를 사용하세요. Storyboards는 유연하고 적응하기 쉬우며, 하나의 storyboard로 모든 launch screen들을 관리할 수 있습니다. 개발자 가이드는 다음의 문서를 참조하세요.



**IMPORTANT** 

Don't use a static image for your launch screen. If you need to know the dimensions of various screen sizes to help you lay out your designs, see [Device Screen Sizes and Orientations](https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/adaptivity-and-layout/#device-screen-sizes-and-orientations).

> Launch screen에 크기가 고정된 이미지를 사용하지 마세요. 디자인의 배치를 위해서 다양한 화면 크기의 치수를 알아야 하는 경우, 다음을 참조하세요.
>
> 



**Design a launch screen that’s nearly identical to the first screen of your app.** If you include elements that look different when the app finishes launching, people can experience an unpleasant flash between the launch screen and the first screen of the app. Also make sure that your launch screen matches the device's current appearance mode; for guidance, see [Dark Mode](https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/dark-mode/).

> **첫 화면과 거의 동일한 launch screen을 디자인하세요.** Launch screen과 첫 화면이 달라 보이면, launch screen이 끝난 후, 사용자들은 그 둘 사이에 불편한 감정을 느낄 수 있습니다. 또한 launch screen이 기기의 현재 appearance 모드와 일치해야 하는 것을 명심하세요. 자세한 내용은 다음 문서를 확인하세요.



**Avoid including text on your launch screen.** Because the content in a launch screen doesn't change, any displayed text won’t be localized.

> **Launch screen에 글자가 포함되는 것을 피하세요.** Launch screen에 있는 콘텐츠는 변경되지 않으므로, 보이는 글자들은 기기에 따라 다르게 적용되지 않습니다. 



**Downplay launch.** People value apps that let them quickly access content and perform tasks. Designing a launch screen that resembles an app’s interface creates the illusion that the app starts instantly. Combined with a fast launch time, this design approach makes your app feel immediately responsive. For a game, the launch screen should transition gracefully into the first screen the game displays.

> **시작을 중요하게 생각하지 마세요.** 사용자들은 앱이 콘텐츠에 빠르게 접근할 수 있고 작업을 수행하는 것을 중요하게 생각합니다. 앱의 인터페이스와 비슷하게 Launch screen을 디자인하는 것은 앱이 즉시 시작하는 것과 같은 환상을 만들어줍니다. 빠른 시작 시간과 결합되어, 이러한 디자인은 앱이 즉시 반응하는 것과 같은 기분이 들도록 합니다. 게임 앱에서, launch screen은 게임이 보이는 첫 화면으로 우아하게 넘어가도록 해야 합니다.



**Don’t advertise.** The launch screen isn’t a branding opportunity. Don’t design an entry experience that looks like a splash screen or an "About" window. Don’t include logos or other branding elements unless they’re a fixed part of your app’s first screen. If your game or other immersive app displays a solid color before transitioning to the first screen, you can create a launch screen that displays only that solid color.

> **광고하지 마세요.** Launch screen은 상표를 광고하는 곳이 아닙니다. 스플래시 화면이나 "정보" 창과 같은 경험을 설계하지 마세요. 앱의 첫 화면에 고정된 부분이 아니라면, 로고나 다른 브랜딩 요소를 포함하지 마세요. 게임이나 다른 전체 화면 앱이 첫 화면으로 넘어가기 전에 단색을 보여준다면, 단색만 보여주는 launch screen을 만들 수 있습니다.