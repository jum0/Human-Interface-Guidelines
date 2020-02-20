# Settings
Some apps may need to provide a way to make setup or configuration choices, but most apps can avoid or delay doing so. Successful apps work well for most people right away, while also offering some convenient ways to adjust the experience. When you design your app to function the way most people expect, you decrease the need for settings.

> 몇몇의 앱들은 설정이나 구성을 선택하는 방식으로 제공해야 할 수 있지만, 대부분의 앱들은 이런 것들을 피하거나 늦출 수 있습니다. 성공적인 앱들은 많은 사용자들에게 즉시 잘 작동하고, 그들이 앱을 사용하면서 겪는 경험들을 조정하는 편리한 방법을 제공합니다. 많은 사용자들이 기대하는 방향으로 기능할 수 있도록 앱을 설계하면, 설정의 필요성은 줄어듭니다.



<img width="271" alt="스크린샷 2020-02-20 오후 11 09 41" src="https://user-images.githubusercontent.com/40762111/74941911-348fdf80-5437-11ea-89da-4c64e7999da4.png">



**Infer what you can from the system.** If you need information about the user, device, or environment, query the system for it whenever possible instead of asking the user. For example, instead of asking someone to enter their zip code so you can present local options, ask permission to use their current location. Gracefully fall back to manual entry if the user denies access to their information.

> **사용자가 시스템으로부터 할 수 있는 것을 추론하세요.** 사용자, 기기, 환경에 관해서 정보가 필요하다면, 사용자에게 묻지 않고 필요할 때마다 시스템에 질문하세요. 예를 들어, 누군가에게 우편 번호 입력을 위해서 부수적인 옵션을 띄워 묻는 대신, 그들의 현재 위치를 이용해도 되는지 허락을 구하세요. 사용자가 그들의 정보에 접근하는 것을 원하지 않는다면, 우아하게 수동으로 입력하는 것으로 돌아가세요.



**Thoughtfully prioritize configuration options within your app.** Your app’s main screen is a good place for options that are essential or that change frequently. Secondary screens are better for options that change only occasionally.

> **앱에서 옵션 구성을 친절하게 우선으로 처리하세요.** 앱의 메인 화면은 필수적이거나 자주 바뀌는 옵션에 적합합니다. 두 번째로 다른 화면들은 오직 가끔 바뀌는 옵션들에 적합합니다.



**Expose infrequently changed configuration options in Settings.** The Settings app is a central location for making configuration changes throughout the system, but people must leave your app to get there. It’s far more convenient to adjust settings directly within your app. If you must provide settings that rarely require change, see [Implementing an iOS Settings Bundle](https://developer.apple.com/library/content/documentation/Cocoa/Conceptual/UserDefaults/Preferences/Preferences.html) in [Preferences and Settings Programming Guide](https://developer.apple.com/library/content/documentation/Cocoa/Conceptual/UserDefaults/Introduction/Introduction.html) for developer guidance.

> **설정에서 드물게 변경되는 구성을 보여주세요.** 

> **설정에서 드물게 변경되는 옵션 구성을 보여주세요.** 설정은 시스템을 전체적으로 변경하는 구성을 만드는 중요한 화면이지만, 사용자가 설정 화면에 가기 위해서는 앱에서 벗어나야만 합니다. 앱 내에서 바로 설정을 변경하는 것이 더 편리합니다. 사용자에게 변경을 거의 요구하지 않는 설정을 제공해야 한다면, 다음 문서들을 확인하세요.

<img width="271" alt="스크린샷 2020-02-20 오후 11 10 07" src="https://user-images.githubusercontent.com/40762111/74941922-39549380-5437-11ea-8267-5fa0e4035bf6.png">

**Provide shortcuts to Settings when appropriate.** If your app includes text that directs users to Settings, such as “Go to Settings > MyApp > Privacy > Location Services,” provide a button that opens that location automatically. For developer guidance, see [openSettingsURLString](https://developer.apple.com/documentation/uikit/uiapplication/1623042-opensettingsurlstring) in [UIApplication](https://developer.apple.com/documentation/uikit/uiapplication).

> 적절한 시기에 설정에 단축키를 제공하세요. 앱에서 "설정으로 가기 > 앱 > 개인 정보 보호 > 위치 서비스" 와 같이 사용자가 설정으로 바로 가는 텍스트를 포함한다면, 위치를 자동으로 열 수 있는 버튼을 제공하세요. 더 많은 정보를 이곳을 확인하세요..

