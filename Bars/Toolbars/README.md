# Toolbars
A toolbar appears at the bottom of an app screen and contains buttons for performing actions relevant to the current view or content within it. Toolbars are translucent, may have a background tint, and often hide when people are unlikely to need them. For example, in Safari, the toolbar hides when you begin scrolling the page since you are likely reading. You can show it again by tapping the bottom of the screen. Toolbars are also hidden when a keyboard is onscreen.

> Toolbar는 앱 화면의 하단에 나타나며, 현재 뷰나 콘텐츠와 관련된 행동들을 수행하는 버튼을 가지고 있습니다. Toolbars는 반투명하며 배경색을 가질 수 있고, 종종 사용자들이 그것들이 필요하지 않을 때 사라집니다. 예를 들어, Safari 앱에서 무언가를 읽기 위해 scrolling을 시작할 때, toolbar는 사라집니다. 화면의 하단을 tap 하여 toolbar가 다시 나타날 수 있도록 할 수 있습니다. Toolbars는 또한 화면에 키보드가 나타날 때 사라지게 됩니다.

<img width="268" alt="스크린샷 2020-03-08 오후 8 09 25" src="https://user-images.githubusercontent.com/40762111/76161669-dc681580-6178-11ea-9330-6009d1daf4d3.png">

**Provide relevant toolbar buttons.** A toolbar should contain frequently used commands that make sense in the current context.

> **Toolbar와 연관된 버튼들을 제공하세요.** Toolbar는 현재 컨텍스트에서 이해되고 빈번하게 사용되는 명령들을 가지고 있어야 합니다.



**Consider whether icons or text-titled buttons are right for your app.** Icons work well when you need more than three toolbar buttons. When you have three buttons or fewer, text can sometimes be clearer. In Calendar, for example, text is used because icons would be confusing. The use of text also allows the Inbox button to show a count of calendar and event invitations.

> **아이콘들 또는 글자로 된 제목 버튼들이 앱에 알맞은지 고려하세요.** 3개보다 많은 toolbar 버튼들이 필요할 때, 아이콘이 더 효과적입니다. 3개 이하의 버튼이 있다면, 때때로 글자가 더 명확할 수 있습니다. 예를 들어, Calendar 앱에서, 아이콘은 혼란을 줄 수 있기 때문에 글자가 사용됩니다. 또한 글자를 사용하면 받은 편지함에서 일정 관리와 이벤트 초대의 수를 표시할 수 있습니다.



**Avoid using a segmented control in a toolbar.** Segmented controls let people switch contexts, whereas a toolbar is specific to the current screen. If you need to provide a way to switch contexts, consider using a tab bar instead. See [Tab Bars](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Bars/Tab%20Bars).

> **Toolbar에서 segmented control 사용하는 것을 피하세요.** Segmented controls는 사용자가 컨텍스트를 전환할 수 있도록 하는 반면, toolbar는 현재 화면에 한정됩니다. 컨텍스트 전환하는 방식을 제공하고자 한다면, toolbar 대신에 tab bar 사용하는 것을 고려하세요. 자세한 내용은 다음 문서를 확인하세요.



**Give text-titled buttons enough room.** If your toolbar includes multiple buttons, the text of those buttons may appear to run together, making the buttons indistinguishable. Add separation by inserting fixed space between the buttons. For developer guidance, see the [UIBarButtonSystemItemFixedSpace](https://developer.apple.com/documentation/uikit/uibarbuttonsystemitem/uibarbuttonsystemitemfixedspace) constant value in [UIBarButtonItem](https://developer.apple.com/documentation/uikit/uibarbuttonitem).

> **글자로 된 버튼은 충분한 여백을 주세요.** Toolbar에 여러 버튼이 있다면, 버튼들의 텍스트는 함께 실행되어 구분되지 않을 수 있습니다. 버튼들 사이에 일정한 공간을 두어 구분되도록 하세요. 개발자 가이드는 다음 문서를 확인하세요.

<img width="268" alt="스크린샷 2020-03-08 오후 8 09 36" src="https://user-images.githubusercontent.com/40762111/76161671-dd994280-6178-11ea-9c3e-3d937d5b91f2.png">

For developer guidance, see [UIToolbar](https://developer.apple.com/documentation/uikit/uitoolbar).

> UIToolbar와 관련된 가이드는 다음 문서를 확인하세요.



**TIP**

It’s important to understand the difference between a toolbar and a tab bar, because both types of bars appear at the bottom of an app screen. A toolbar contains buttons for performing actions related to the current context, such as creating an item, deleting an item, adding an annotation, or taking a photo. A tab bar lets the user switch quickly between different sections of an app, for example, the Alarm, Stopwatch, and Timer tabs in the Clock app. See [Tab Bars](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Bars/Tab%20Bars). Toolbars and tab bars never appear together in the same view.

> Toolbar와 tab bar는 모두 화면의 하단에 나타나기 때문에, 차이점을 이해하는 것이 중요합니다. Toolbar는 현재 컨텍스트와 관련된 기능을 수행하는 버튼을 가지고 있는데, item을 만들거나 삭제하고 주석을 추가하거나 사진을 찍는 것들이 있습니다. Tab bar는 사용자가 화면의 다른 섹션을 빠르게 이동할 수 있도록 도와주는데, Clock 앱의 Alarm, Stopwatch, Timer tabs과 같은 것들이 있습니다. 자세한 내용은 문서를 확인해주세요. Toolbars와 tab bars는 절대로 같은 view에 나타나지 않습니다.