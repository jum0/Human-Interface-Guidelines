# Navigation
People tend to be unaware of an app’s navigation until it doesn’t meet their expectations. Your job is to implement navigation in a way that supports the structure and purpose of your app without calling attention to itself. Navigation should feel natural and familiar, and shouldn’t dominate the interface or draw focus away from content. In iOS, there are three main styles of navigation.

> 사용자들은 앱이 그들의 기대에 미치지 못할 때까지 앱의 내비게이션에 대해 알지 못하는 경향이 있습니다. 따라서 주의를 따로 환기시키지 않고 앱의 구조와 목적으로 지원하는 방식으로 내비게이션을 구현합니다. 내비게이션은 자연스럽고 익숙해야 하며, 인터페이스보다 집중되거나 콘텐츠로부터 집중하지 못하게 해서는 안 됩니다. iOS에서는 내비게이션의 3가지 주요 스타일이 있습니다.



#### Hierarchical Navigation

Make one choice per screen until you reach a destination. To go to another destination, you must retrace your steps or start over from the beginning and make different choices. Settings and Mail use this navigation style.

> 사용자가 어떤 화면에 도달하기 전까지 각 화면에서 한 가지 선택을 하도록 합니다. 또 다른 화면으로 이동하기 위해서는, 사용자는 이동했던 경로를 뒤짚어가거나 처음부터 다시 시작하여 다른 선택을 해야합니다. 설정이나 메일이 이러한 내비게이션 방식을 사용합니다.

<img width="368" alt="navigation1" src="https://user-images.githubusercontent.com/40762111/74616192-bea32400-5169-11ea-9ed9-72e1603454a4.png">

#### Flat Navigation

Switch between multiple content categories. Music and App Store use this navigation style.

> 다수의 콘텐츠 카테고리 사이에서 화면을 전환합니다. 음악이나 앱스토어가 이러한 내비게이션 방식을 사용합니다.

<img width="364" alt="navigation2" src="https://user-images.githubusercontent.com/40762111/74616190-be0a8d80-5169-11ea-841f-0876afcf97c2.png">



#### Content-Driven or Experience-Driven Navigation

Move freely through content, or the content itself defines the navigation. Games, books, and other immersive apps generally use this navigation style.

> 여러 콘텐츠 사이에 자유롭게 이동하거나 콘텐츠 그 자체가 내비게이션으로 정의됩니다. 게임, 책 그리고 다른 전체 화면을 사용하는 앱들이 일반적으로 이런 내비게이션 방식을 사용합니다.

<img width="560" alt="navigation3" src="https://user-images.githubusercontent.com/40762111/74616185-bba83380-5169-11ea-91a1-16e9c4311b57.png">

Some apps combine multiple navigation styles. For example, an app that uses flat navigation may implement hierarchical navigation within each category.

> 몇몇의 앱들은 여러 개의 내비게이션 방식을 결합합니다. 예를 들어서, flat 내비게이션 방식을 이용하는 앱이 각 카테고리 안에서는 hierarchical 내비게이션 방식을 구현할 수 있습니다.



**Always provide a clear path.** People should always know where they are in your app and how to get to their next destination. Regardless of navigation style, it’s essential that the path through content is logical, predictable, and easy to follow. In general, give people one path to each screen. If they need to see a screen in multiple contexts, consider using an action sheet, alert, popover, or modal view. To learn more, see [Action Sheets](https://developer.apple.com/design/human-interface-guidelines/ios/views/action-sheets/), [Alerts](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Views/Alerts), [Popovers](https://developer.apple.com/design/human-interface-guidelines/ios/views/popovers/), and [Modality](https://github.com/jum0/Human-Interface-Guidelines/tree/master/App%20Architecture/Modality).

> **항상 명확한 이동 경로를 제공하세요.** 사용자들은 항상 자신이 앱에서 어디에 있는지, 다른 화면으로 이동하기 위해서는 어떻게 해야 하는지 알고 있어야 합니다. 내비게이션 방식에 상관없이, 콘텐츠를 통한 이동 경로는 논리적이며 예측할 수 있어야 하고 쉽게 알아차릴 수 있어야 합니다. 일반적으로, 사용자에게 각 화면에서 하나의 이동 경로를 제공하세요. 사용자가 여러 환경에서 한 화면을 보고 싶어 한다면, action sheet나, alert, popover, 또는 modal view를 고려하세요. 더 많은 정보는 여기서 얻을 수 있습니다.



**Design an information structure that makes it fast and easy to get to content.** Organize your information structure in a way that requires a minimum number of taps, swipes, and screens.

> **콘텐츠에 빠르고 쉽게 접근하기 위해서 IA(정보 구조)를 설계하세요.** 최소한의 taps, swipes, 화면의 개수로 IA를 구조화하세요. 



**Use touch gestures to create fluidity.** Make it easy to move through your interface with minimum friction. For example, you could let people swipe from the side of the screen to return to the previous screen.

> **우아하게 만들기 위해서 터치 제스처를 이용하세요.** 최소한의 방해로 인터페이스를 이동하기 쉽게 만드세요. 예를 들어, 사용자가 화면의 가장 자리에서 스와이프 하여 이전 화면으로 돌아갈 수 있도록 할 수 있습니다.



**Use standard navigation components.** Whenever possible, use standard navigation controls such as page controls, tab bars, segmented controls, table views, collection views, and split views. Users are already familiar with these controls, and will intuitively know how to get around your app.

> **표준화된 내비게이션 요소들을 이용하세요.** 가능하다면, page controls, tab bars, segmented controls, table views, collection views, split views 등과 같이 표준화된 내비게이션 control들을 사용하세요. 사용자들은 이미 이러한 control 들에 익숙하고, 직관적으로 앱의 구조를 파악할 수 있을 것입니다.
>
> 참조 [iOS 13 Segmented Control](https://packages.framer.com/package/tes/ios-13-segmented-control)



**Use a navigation bar to traverse a hierarchy of data.** The navigation bar’s title can show the current position in the hierarchy, and the back button makes it easy to return to the previous location. For specific guidance, see [Navigation Bars](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Bars/Navigation%20Bars).

> 계층화된 데이터를 이용하기 위해서 내비게이션 bar를 이용하세요. 내비게이션 bar의 제목은 계층적인 구조에서 현재의 위치를 보여줄 수 있고, 뒤로 가기 버튼은 이전 화면으로 돌아갈 수 있도록 도와줍니다. 자세한 내용은 여기에서 확인할 수 있습니다.



**Use a tab bar to present peer categories of content or functionality.** A tab bar lets people quickly and easily switch between categories, regardless of the current location. For specific guidance, see [Tab Bars](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Bars/Tab%20Bars).

> **콘텐츠나 기능적으로 비슷한 카테고리를 나타내기 위해서 tab bar를 사용하세요.** 사용자들은 Tab bar를 통해서 현재의 화면 위치에 상관없이, 카테고리 간에 쉽고 빠르게 이동할 수 있습니다. 자세한 내용은 여기에서 확인할 수 있습니다.



**Use a page control when you have multiple pages of the same type of content.** A page control clearly communicates the number of pages available and which one is currently active. The Weather app uses a page control to show location-specific weather pages. For specific guidance, see [Page Controls](https://developer.apple.com/design/human-interface-guidelines/ios/controls/page-controls/).

> **같은 종류의 콘텐츠를 갖고 있는 화면이 여러 개라면 page control을 사용하세요.** Page control은 현재 어떤 화면에 있고, 몇 개의 페이지를 이용할 수 있는지 명확하게 알려줍니다. 날씨 앱은 구체적인 장소의 날씨 페이지를 보여주기 위해서 page control을 사용합니다. 자세한 내용은 여기에서 확인할 수 있습니다.



**TIP** 

Segmented controls and toolbars don’t enable navigation. Use a segmented control to organize information into different categories. Use a toolbar to provide controls for interacting with the current context. For additional information on these types of elements, see [Segmented Controls](https://developer.apple.com/design/human-interface-guidelines/ios/controls/segmented-controls/) and [Toolbars](https://developer.apple.com/design/human-interface-guidelines/ios/bars/toolbars/).

> segmented control과 toolbar는 내비게이션을 사용할 수 없도록 합니다. 정보를 다른 카테고리로 묶기 위해서segmented control을 사용하세요. 현재 context에서 인터랙팅하기 위한 control을 제공하기 위해서 툴바를 사용하세요. 더 많은 정보와 이러한 요소들의 종류는 여기에서 확인할 수 있습니다.