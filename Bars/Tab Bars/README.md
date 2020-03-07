# Tab Bars
A tab bar appears at the bottom of an app screen and provides the ability to quickly switch between different sections of an app. Tab bars are translucent, may have a background tint, maintain the same height in all screen orientations, and are hidden when a keyboard is displayed. A tab bar may contain any number of tabs, but the number of visible tabs varies based on the device size and orientation. If some tabs can’t be displayed due to limited horizontal space, the final visible tab becomes a More tab, which reveals the additional tabs in a list on a separate screen.

> Tab bar는 앱 화면의 하단에 위치하고 앱에서 서로 다른 섹션으로 빠르게 이동할 수 있도록 도와줍니다. Tab bars는 반투명하지만 배경 색을 가질 수도 있고, 가로와 세로 화면에서 같은 높이를 가집니다. 그리고 키보드가 나타나면 사라집니다. Tab bar는 여러 개의 tabs을 가질 수 있지만, 기기의 크기와 방향에 따라 보이는 tab의 수는 다양합니다. 만약 몇 개의 tabs이 한정된 공간으로 보일 수 없다면, 마지막으로 보이는 tab은  더 보기(More) tab이 되어 별도의 화면에 나머지 tabs의 목록이 나타납니다.



<img width="268" alt="스크린샷 2020-03-07 오후 10 35 40" src="https://user-images.githubusercontent.com/40762111/76144458-07dcf880-60c4-11ea-912a-30945f70f7ec.png">

**In general, use a tab bar to organize information at the app level.** A tab bar is a good way to flatten your information hierarchy and provide access to several peer information categories or modes at once.

> **일반적으로, 앱 레벨에서의 정보를 구성하기 위해서 tab bar를 사용하세요.** Tab bar는 정보 계층을 일정하게 만들기 좋은 방법이고, 동등한 정보 범주나 모드에 한 번에 접근할 수 있도록 합니다.



**Use a tab bar strictly for navigation.** Tab bar buttons should not be used to perform actions. If you need to provide controls that act on elements in the current view, use a toolbar instead. See [Toolbars](https://developer.apple.com/design/human-interface-guidelines/ios/bars/toolbars/).

> **Navigation에서 tab bar를 정확하게 사용하세요.** Tab bar 버튼들은 어떠한 행동을 수행하기 위해서 사용되어서는 안됩니다. 현재의 뷰의 elements에 영향을 주는 제어가 필요하다면, Tab bar 대신에 toolbar를 사용하세요. 자세한 내용은 다음 문서를 확인하세요.



**Avoid having too many tabs.** Each additional tab reduces the tappable area for selecting a tab and increases the complexity of your app, making it harder to locate information. Although a More tab can display extra tabs, this requires additional taps and is a poor use of space. Include essential tabs only, and use the minimum tabs necessary for your information hierarchy. Too few tabs can be a problem too, as it can make your interface appear disconnected. In general, use between three and five tabs on iPhone. A few more are acceptable on iPad.

> **너무 많은 tabs 넣는 것을 피하세요.** 각 추가 tab은 탭 선택을 위한 tap이 가능한 영역을 감소시키고, 정보를 배치하기 어렵게 만들어 앱을 복잡하게 만듭니다. 더 보기(More) tab은 따른 tabs을 보여줄 수 있지만, 추가적인 tap이 필요하고 공간의 사용을 부족하게 만듭니다. 필수적인 tabs만 포함하고, 정보 계층에서 필요한 최소한의 tabs만 사용하세요. Tabs이 거의 없는 것도 인터페이스가 분리되어 보일 수 있기 때문에 문제가 될 수 있습니다. 일반적으로 아이폰에서는 3개에서 5개 사이의 tabs을 사용합니다. iPad에서는 조금 더 많습니다.



**Don't hide a tab bar when people navigate to different areas in your app.** A tab bar enables global navigation for your app, so it should remain visible everywhere. The exception to this is in modal views. Because a modal view gives people a separate experience that they dismiss when they're finished, it's not part of the overall navigation of your app.

> **사용자가 앱의 다른 영역으로 이동할 때, tab bar를 숨기지 마세요.** Tab bar는 앱에서 전체적으로 이동할 수 있도록 도와주기 때문에, 어느 곳에 있든지 보여야 합니다. model view에서는 예외입니다. Model view는 사용자가 작업을 마쳤을 때 그것을 무시하는 분리된 경험을 주기 때문에, 그것은 앱에서 전체적인 내비게이션 부분이 아닙니다.



**Don’t remove or disable a tab when its function is unavailable.** If tabs are available in some cases but not in others, your app’s interface becomes unstable and unpredictable. Ensure that all tabs are always enabled, and explain why a tab’s content is unavailable. For example, if there are no songs on an iOS device, the My Music tab in the Music app explains how to download songs.

> **Tab의 기능을 이용할 수 없을 때, tab을 제거하거나 사용할 수 없도록 하지 마세요.** Tabs이 몇 가지 상황에서만 사용 가능하다면, 앱의 인터페이스는 불안정하고 예상하지 못하게 됩니다. 항상 모든 tabs을 사용할 수 있도록 유지하고, tab의 콘텐츠를 사용하지 못하는 이유를 설명해 주세요. 예를 들어, iOS 기기에 노래가 없다면, Music 앱의 My Music tab에서 노래 다운로드하는 방법을 설명해 주세요.



**Always switch contexts in the attached view.** To keep your interface predictable, selecting a tab should always affect the view that’s directly attached to the tab bar, not another view elsewhere on screen. For example, selecting a tab on the left side of a split view shouldn’t cause the right side of the split view to suddenly change. Selecting a tab in a popover shouldn’t cause the view behind the popup to change.

> **항상 연관된 view의 contexts를 전환하세요.** 예상 가능한 인터페이스를 구성하기 위해서는, tab을 선택했을 때 화면의 또 다른 view가 아닌, tab bar에 직접적으로 관련된 view에 영향을 주어야 합니다. 예를 들어, 분할된 view의 왼쪽에 부분에 있는 tab을 선택했다면, 분할된 view의 오른쪽에 갑자기 변경되지 않아야 합니다. Popover에서 tab을 선택했다면 popup 뒤의 뷰가 변경되지 않아야 합니다.



**Make sure tab bar icons are visually consistent and balanced.** The system offers a range of predefined icons for common use cases. See [System Icons > Tab Bar Icons](https://developer.apple.com/design/human-interface-guidelines/ios/icons-and-images/system-icons/#tab-bar-icons). You can also create your own icons. See [Custom Icons](https://developer.apple.com/design/human-interface-guidelines/ios/icons-and-images/custom-icons/).

> **Tab bar의 아이콘들은 시각적으로 통일성을 지니며 균형 있어야 한다는 것을 명심하세요.** 시스템에서는 다양한 상황을 대비하여 이미 만들어진 아이콘들을 제공합니다. 다음 문서를 확인해 보세요. 또한 새로운 아이콘도 만들 수 있습니다. 관련된 내용은 다음 문서를 확인해 보세요.



**Use badging to communicate unobtrusively.** You can display a badge—a red oval containing white text and either a number or an exclamation point—on a tab to indicate that new information is associated with that view or mode.

> **드러나지 않게 의사소통하기 위해서 badging을 사용하세요.** Tab 안에 view 또는 mode와 관련된 새로운 정보가 있다는 것을 알려주기 위해서 빨간 원 안의 하얀 텍스트와 숫자 또는 느낌표의 badge를 보여줄 수 있습니다.



For developer guidance, see [UITabBar](https://developer.apple.com/documentation/uikit/uitabbar).

> 자세한 개발자 가이드는 다음 문서를 확인해 보세요.



**TIP**

It’s important to understand the difference between a tab bar and a toolbar, because both types of bars appear at the bottom of an app screen. A tab bar lets the user switch quickly between different sections of an app, such as the Alarm, Stopwatch, and Timer tabs in the Clock app. A toolbar contains buttons for performing actions related to the current context, like creating an item, deleting an item, adding an annotation, or taking a photo. See [Toolbars](https://developer.apple.com/design/human-interface-guidelines/ios/bars/toolbars/). Tab bars and toolbars never appear together in the same view.

> Tab bar와 toolbar는 모두 화면의 하단에 나타나기 때문에, 차이점을 이해하는 것이 중요합니다. Tab bar는 사용자가 화면의 다른 섹션을 빠르게 이동할 수 있도록 도와주는데, Clock 앱의 Alarm, Stopwatch, Timer tabs과 같은 것들이 있습니다. Toolbar는 현재 컨텍스트와 관련된 기능을 수행하는 버튼을 가지고 있는데, item을 만들거나 삭제하고 주석을 추가하거나 사진을 찍는 것들이 있습니다. 자세한 것은 문서를 확인해 주세요. Tab bars와 toolbars는 절대로 같은 view에서 나타나지 않습니다.

