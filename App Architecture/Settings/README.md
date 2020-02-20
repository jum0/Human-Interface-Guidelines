# Settings
Some apps may need to provide a way to make setup or configuration choices, but most apps can avoid or delay doing so. Successful apps work well for most people right away, while also offering some convenient ways to adjust the experience. When you design your app to function the way most people expect, you decrease the need for settings.

> 몇몇의 앱들은 설정이나 구성을 선택하는 방식으로 제공해야 할 수 있지만, 대부분의 앱들은 이런 것들을 피하거나 늦출 수 있습니다. 성공적인 앱들은 많은 사용자들에게 즉시 잘 작동하고, 그들이 앱을 사용하면서 겪는 경험들을 조정하는 편리한 방법을 제공합니다. 많은 사용자들이 기대하는 방향으로 기능할 수 있도록 앱을 설계하면, 설정의 필요성은 줄어듭니다.



<img width="271" alt="스크린샷 2020-02-20 오후 11 09 41" src="https://user-images.githubusercontent.com/40762111/74941911-348fdf80-5437-11ea-89da-4c64e7999da4.png">



**Infer what you can from the system.** If you need information about the user, device, or environment, query the system for it whenever possible instead of asking the user. For example, instead of asking someone to enter their zip code so you can present local options, ask permission to use their current location. Gracefully fall back to manual entry if the user denies access to their information.

> **사용자가 시스템으로부터 할 수 있는 것을 추론하세요.** 사용자, 기기, 환경에 관해서 정보가 필요하다면, 사용자에게 묻지 않고 가능할 때마다 시스템에 문의하세요. 예를 들어, 



**Thoughtfully prioritize configuration options within your app.** Your app’s main screen is a good place for options that are essential or that change frequently. Secondary screens are better for options that change only occasionally.

> ㅇㄹㅇㄹㅇㄹㅇㄹ



**Expose infrequently changed configuration options in Settings.** The Settings app is a central location for making configuration changes throughout the system, but people must leave your app to get there. It’s far more convenient to adjust settings directly within your app. If you must provide settings that rarely require change, see [Implementing an iOS Settings Bundle](https://developer.apple.com/library/content/documentation/Cocoa/Conceptual/UserDefaults/Preferences/Preferences.html) in [Preferences and Settings Programming Guide](https://developer.apple.com/library/content/documentation/Cocoa/Conceptual/UserDefaults/Introduction/Introduction.html) for developer guidance.

> ㅇㄹㅇㄹㅇㄹㅇㄹ



<img width="271" alt="스크린샷 2020-02-20 오후 11 10 07" src="https://user-images.githubusercontent.com/40762111/74941922-39549380-5437-11ea-8267-5fa0e4035bf6.png">

**Provide shortcuts to Settings when appropriate.** If your app includes text that directs users to Settings, such as “Go to Settings > MyApp > Privacy > Location Services,” provide a button that opens that location automatically. For developer guidance, see [openSettingsURLString](https://developer.apple.com/documentation/uikit/uiapplication/1623042-opensettingsurlstring) in [UIApplication](https://developer.apple.com/documentation/uikit/uiapplication).

> ㅇㄹㅇㄹㅇㄹ

