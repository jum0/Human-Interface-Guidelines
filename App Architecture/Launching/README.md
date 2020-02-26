# Launching
The launch experience has a significant impact on the way people feel about your app. Regardless of the device people are using or how long it's been since they last opened your app, the launch experience should be fast and seamless.

> 시작 화면의 경험은 사용자들이 앱에 대해서 느끼는 방식에 중요한 영향을 미칩니다. 사용자들이 사용하는 기기나 그들이 어플을 마지막을 켠지 얼마나 되었는지에 관계없이, 시작 화면의 경험은 빠르고 매끄러워야 합니다.



The guidelines below can help you design a delightful launch experience. For developer guidance, see [Responding to the Launch of Your App](https://developer.apple.com/documentation/uikit/app_and_environment/responding_to_the_launch_of_your_app).

> 아래의 가이드라인은 기분 좋은 시작 화면의 경험을 설계하는 데 도움을 줄 수 있습니다. 개발자 가이드라인은 다음을 참조하세요. 



**Provide a launch screen.** The system displays your launch screen the moment your app starts and quickly replaces it with your app's first screen. The function of a launch screen is to give people the impression that your app is fast and responsive, while allowing initial content to load. To ensure a seamless transition from your launch screen, design a plain screen that resembles your first app screen and doesn't draw attention to itself. For guidance, see [Launch Screen](https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/launch-screen).

> **시작 화면을 제공하세요.** 시스템은 앱이 시작하고 빠르게 처음 화면으로 바뀌는 순간, 시작 화면을 보여줍니다. 시작 화면의 기능은 초기의 콘텐츠가 준비되는 동안에, 사용자에게 앱이 빠르고 즉각 반응한다는 인상을 주는 것입니다. 시작 화면에서의 매끄러운 화면 이동을 위해서, 앱의 첫 번째 화면과 비슷하게 단순한 화면을 설계하고, 그 화면 자체에 관심을 끌도록 하지 마세요. 자세한 가이드는 다음을 확인하세요.



**Launch in the appropriate orientation.** If your app supports both portrait and landscape modes, it should launch using the device’s current orientation. If your app only runs in one orientation, it should always launch in that orientation and let people rotate the device if necessary. Unless there’s a compelling reason not to, an app in landscape mode should orient itself correctly, regardless of whether the device was rotated left or right. For guidance, see [Adaptivity and Layout](https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/adaptivity-and-layout).

> **적절한 방향에서 시작하세요.** 앱이 세로 모드와 가로 모드를 모두 지원한다면, 시작 화면은 기기의 현재 방향을 사용해야 합니다. 앱이 가로와 세로 둘 중 한 가지 모드에서만 실행된다면, 시작 화면은 항상 그 모드에서만 시작해야 하고 필요하다면 사용자가 화면(기기)을 돌릴 수 있도록 해야 합니다. 꼭 그렇게 하지 않아야 하는 이유가 없다면 기기를 왼쪽이나 오른쪽으로 회전하는 것에 관계없이, 가로 모드에 있는 앱은 방향을 올바르게 조정해야 합니다.



**Avoid asking for setup information up front.** People expect apps to just work. Design your app for the majority of users and let the few that want a different configuration adjust settings to meet their needs. As much as possible, get setup information from device settings and defaults, or through a synchronization service, such as iCloud. If you must ask for setup information, prompt people to supply it the first time they open the app, and let them modify it later in your app’s settings.

> **미리 설정 정보를 묻는 것을 피하세요.** 사용자들은 앱이 단지 작동하는 것을 기대합니다. 다수의 사용자들을 위해서 앱을 설계하고, 소수의 사용자들이 그들의 니즈를 위해 다른 설정을 조정할 수 있도록 하세요. 가능한 한, 기기의 설정 및 기본 값이나 iCloud와 같은 동기화 서비스를 통해 설정 정보를 얻으세요. 설정 정보를 물어야만 한다면, 사용자가 어플을 처음 실행할 때, 제공하도록 하고 나중에 설정에서 변경할 수 있도록 하세요.



**Avoid showing in-app licensing agreements and disclaimers.** Let the App Store display agreements and disclaimers so people can read them before downloading your app. If you must include these items within the app, integrate them in a balanced way that doesn’t disrupt the user experience.

> **앱 내에서 라이선스에 동의하거나 거부하는 것을 보이지 않도록 하세요.** 앱 스토어에 동의나 거부를 표시하여, 사용자들이 앱을 다운로드하기 전에 그것들을 읽을 수 있도록 하세요. 이러한 것들을 앱에 포함해야만 한다면, 사용자 경험을 해치지 않는 방식으로 균형을 맞추어 통합하세요.



**Restore the previous state when your app restarts.** Don't make people retrace steps to reach their previous location in your app. Preserve and restore your app’s state so they can continue where they left off.

> **앱을 다시 시작할 때, 이전의 상태를 저장하세요.** 사용자가 앱에서 이전의 위치를 알기 위해서 돌아가 확인하도록 하지 마세요. 사용자가 앱에서 그만둔 지점에서 다시 계속할 수 있도록 앱의 상태를 유지하고 저장하세요.



**Don’t encourage rebooting.** Restarting takes time and makes your app seem unreliable and hard to use. If your app has memory or other issues that make it difficult to run unless the system has just booted, you need to address those issues.

> **앱을 껐다가 다시 켜지 않도록 한세요.** 앱을 다시 켜는 것은 시간이 소요되고, 신뢰할 수 없거나 사용하기 어려워 보이도록 합니다. 시스템이 다시 부팅되지 않는 한 앱이 실행하기 어려운 메모리나 다른 문제를 가지고 있다면, 그러한 문제들을 해결할 필요가 있습니다.



**Avoid asking people to rate your app too quickly or too often.** Asking for a rating soon after first launch — or too frequently while people are using your app — is annoying and likely to decrease the amount of useful feedback you receive. To encourage well-considered feedback, give people time to form an opinion about your app before asking for a rating. Always provide a way to opt out of rating prompts and never force people to rate your app.

> **사용자에게 앱을 너무 일찍 또는 자주 평가하도록 묻는 것을 피하세요.** 사용자에게 앱을 처음 실행하거나 사용 중에 빈번하게 평가를 요구하는 것은 그들을 귀찮게 하거나 유의미한 피드백의 수를 줄일 수 있습니다. 사용자에게 평가를 요청하기 앞서서 의미 있는 피드백을 얻기 위해는 앱에 대한 생각을 가질 수 있도록 시간을 주어야 합니다. 항상 즉각적인 평가를 하지 않는 방식으로 제공하고, 사용자에게 앱에 대한 평가를 하도록 강요하지 마세요.