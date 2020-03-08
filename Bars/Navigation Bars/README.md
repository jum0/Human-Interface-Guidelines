# Navigation Bars
A navigation bar appears at the top of an app screen, below the status bar, and enables navigation through a series of hierarchical screens. When a new screen is displayed, a back button, often labeled with the title of the previous screen, appears on the left side of the bar. Sometimes, the right side of a navigation bar contains a control, like an Edit or a Done button, for managing the content within the active view. In a split view, a navigation bar may appear in a single pane of the split view. Navigation bars are translucent, may have a background tint, and can be configured to hide when the keyboard is onscreen, a gesture occurs, or a view resizes.

> 내비게이션 바는 앱 화면의 최상단, 상태 바 아래에 나타나고, 계층적인 화면들을 통해 탐색이 가능하도록 합니다. 새로운 화면이 보인다면 보통 뒤로 가기 버튼은 이전 화면의 제목으로 붙여지고, 내비게이션 바의 왼쪽에 나타납니다. 때때로, 내비게이션 바의 오른쪽 부분은 활성화된 뷰에서 콘텐츠를 관리하기 위해서 편집, 완료 버튼과 같은 컨트롤 버튼을 포함합니다. 분할된 화면에서, 내비게이션 바는 분할된 화면의 하나에 나타날 수도 있습니다. 내비게이션 바는 반투명이고 배경색을 가질 수 있으며, 키보드가 화면에 보일 때, 제스처가 발생할 때, 화면의 크기를 조정할 때 숨길 수 있습니다.

<img width="284" alt="스크린샷 2020-02-19 오전 9 33 05" src="https://user-images.githubusercontent.com/40762111/74790457-eecdfc80-52fa-11ea-9151-5f1e23190b08.png">



**Consider temporarily hiding the navigation bar when displaying full-screen content.** The navigation bar can be distracting when you want to focus on content. Temporarily hide the bar to provide a more immersive experience. Photos hides the navigation bar and other interface elements when viewing full-screen photos. If you implement this type of behavior, let people restore the navigation bar with a simple gesture, like a tap.

> **전체 화면으로 콘텐츠를 보여줄 때, 일시적으로 내비게이션 바 숨기는 것을 고려하세요.** 내비게이션 바는 사용자가 콘텐츠에 집중하고자 할 때, 주의를 분산시킬 수 있습니다. 사용자가 온전히 집중할 수 있는 경험을 제공하기 위해서 일시적으로 내비게이션 바를 숨기세요. 사진 애플리케이션은 사진을 전체 화면으로 볼 때, 내비게이션 바와 다른 인터페이스 요소들을 보이지 않게 합니다. 이런 종류의 행동을 추가한다면, 사용자가 tap과 같은 간단한 제스처로 내비게이션 바가 다시 보이도록 하세요.



For developer guidance, see [UINavigationBar](https://developer.apple.com/documentation/uikit/uinavigationbar).

> 개발자 가이드는 이곳을 확인하세요.



**TIP**

Use a toolbar when navigation isn’t needed or you want multiple controls for managing content. See [Toolbars](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Bars/Toolbars).

> 내비게이션이 필요하지 않거나, 콘텐츠를 관리하기 위해서 다중의 컨트롤을 원한다면 툴바를 사용하세요. 툴바는 여기서 확인할 수 있습니다.



## Navigation Bar Titles

**Consider showing the title of the current view in the navigation bar.** In most cases, a title helps people understand what they’re looking at. However, if titling a navigation bar seems redundant, you can leave the title empty. For example, Notes doesn’t title the current note because the first line of content supplies all the context needed.

> **내비게이션 바에 현재 화면의 제목 띄우는 것을 고려하세요.** 대부분의 경우, 제목은 사용자가 보고 있는 것이 무엇인지 도와줍니다. 하지만, 내비게이션 바의 제목이 불필요한 것처럼 느껴진다면, 빈 공간을 남겨둘 수 있습니다. 예를 들어, 메모장 애플리케이션은 현재 메모에 제목을 붙이지 않았습니다. 그 이유는 콘텐츠의 첫 번째 줄이 콘텐츠가 필요한 모든 정보를 제공하고 있기 때문입니다.



<img width="569" alt="스크린샷 2020-02-19 오전 9 37 08" src="https://user-images.githubusercontent.com/40762111/74790638-859ab900-52fb-11ea-9ecd-3d399297efba.png">



**Use a large title when you want to provide extra emphasis on context.** Large titles should never compete with content, but in some apps, the big, bold text of a large title can help orient people as they browse and search. In a tabbed layout, for example, large titles can help clarify the active tab and indicate when people have scrolled to the top. Phone uses this approach, while Music uses large titles to differentiate content areas like albums, artists, playlists, and radio. In iOS 13 and later, a large title navigation bar doesn’t include a background material or shadow by default. Also, a large title transitions to a standard title as people begin scrolling the content. For developer guidance, see [prefersLargeTitles](https://developer.apple.com/documentation/uikit/uinavigationbar/2908999-preferslargetitles).

> **화면의 컨텍스트를 더 강조하고 싶다면 큰 제목을 사용하세요.** 큰 제목이 절대 콘텐츠를 흐려서는 안됩니다. 하지만, 몇몇 앱에서 크고 두꺼운 폰트의 제목은 사용자가 훑어보고 검색할 때, 자신들의 위치를 알 수 있도록 돕습니다. 예를 들어 tab으로 구성된 레이 아웃에서, 큰 제목은 활성화된 tab을 명확히 하는 데 도움을 줄 수 있고 사용자가 맨 위쪽으로 스크롤 할 때 나타납니다. 전화 애플리케이션은 이러한 구성을 사용하지만, 음악 애플리케이션은 앨범, 가수, 재생 목록, 라디오와 같은 영역을 콘텐츠와 구분하기 위해서 큰 제목을 사용합니다. iOS 13 이상의 버전에서는 내비게이션 바의 큰 제목이 기본적으로 배경 요소나 그림자를 포함하고 있지 않습니다. 또한, 사용자들이 콘텐츠를 스크롤링 할 때, 큰 제목에서 기본 제목으로 변경되지 않습니다. 개발자 가이드는 다음을 확인하세요.



**Consider hiding the border of a large-title navigation bar.** In iOS 13 and later, you can hide the bottom border of a navigation bar by removing the bar’s shadow (the border automatically reappears when people scroll the content area). The borderless style works well in large-title navigation bars because it enhances the sense of connection between title and content. The borderless style may not work as well in standard-title navigation bars, though, because the bar’s title and buttons might be harder to distinguish. An exception to this is in a split view on iPad: You might want to maintain consistency between the master and detail views by using the borderless style in both.

> **큰 제목의 내비게이션 바의 경계는 숨기는 것을 고려하세요** iOS 13 이상의 버전에서는 내비게이션 바의 그림자를 숨김으로써 아래쪽 경계를 숨길 수 있습니다(사용자가 콘텐츠 영역을 스크롤 하면 경계는 다시 드러납니다.) 경계가 없는 스타일은 큰 제목의 내비게이션 바에 적합합니다. 그 이유는 제목과 콘텐츠 사이의 감성(sense)을 향상시킬 수 있기 때문입니다. 그럼에도 불구하고, 이런 스타일은 기본적인 제목의 내비게이션 바에는 적합하지 않을 수 있습니다. 왜냐하면 내비게이션 바의 제목과 버튼을 구별하기 더 어려워질 수 있기 때문입니다. 아이패드의 분할된 화면은 예외로, 주화면과 보조 화면 양쪽 모두에 경계가 없는 스타일을 사용함으로써 두 화면 간 일관성을 유지하고 싶을 것입니다.
>
> 



## Navigation Bar Controls

**Avoid crowding a navigation bar with too many controls.** In general, a navigation bar should contain no more than the view’s current title, a back button, and one control that manages the view’s contents. If you use a segmented control in the navigation bar, the bar shouldn’t include a title or any controls other than the segmented control.

> **너무 많은 control들로 내비게이션 바가 복잡해지는 것을 피하세요.** 일반적으로, 내비게이션 바는 화면의 현재 제목, 뒤로 가기 버튼, 화면의 콘텐츠들을 관리하는 하나의 control만 포함해야 합니다. 내비게이션 바에 segmented control을 사용한다면, segmented control 이외의 제목이나 control이 포함되어서는 안됩니다.



**Use the standard back button.** People know that the standard back button lets them retrace steps through a hierarchy of information. However, if you implement a custom back button, make sure it still looks like a back button, behaves intuitively, matches the rest of your interface, and is consistently implemented throughout your app. If you replace the system-provided back button chevron with a custom image, supply a custom mask image too. iOS uses this mask to animate the button title during transitions.

> **기본의 뒤로 가기 버튼을 사용하세요.** 사용자들은 계층적인 정보에서 기본적인 뒤로 가기 버튼을 통해 이전으로 돌아가는 것을 알고 있습니다. 하지만, custom된 뒤로 가기 버튼을 사용하고자 한다면, 뒤로 가기 버튼과 비슷해야 하며, 직관적으로 알아볼 수 있고, 다른 인터페이스들과 어울리며, 앱의 전체적인 부분에서 일관성을 유지해야 합니다. 기본적으로 제공되는 V자 모양 뒤로 가기 버튼을 custom 이미지로 변경한다면, custom mask 이미지도 추가하세요. iOS는 이러한 mask를 버튼의 제목이 변경되는 동안 움직이는데 사용합니다.



**Don’t include multisegment breadcrumb paths.** The back button always performs a single action—returning to the previous screen. If you think people might get lost without the full path to the current screen, consider flattening your app’s hierarchy.

> **multisegment breadcrumb path들을 포함하지 마세요** 뒤로 가기 버튼은 항상 이전 화면으로 돌아가는 하나의 행동만을 수행합니다. 사용자가 현재 화면에서 전체적인 진행을 알려주는 것이 없어 헤맬 수 있다고 생각되면, 앱의 계층적인 구조를 보완하세요.



**Give text-titled buttons enough room.** If your navigation bar includes multiple text buttons, the text of those buttons may appear to run together, making the buttons indistinguishable. Add separation by inserting a fixed space item between the buttons. For developer guidance, see the [UIBarButtonSystemItemFixedSpace](https://developer.apple.com/documentation/uikit/uibarbuttonsystemitem/uibarbuttonsystemitemfixedspace) constant value in [UIBarButtonItem](https://developer.apple.com/documentation/uikit/uibarbuttonitem).

> **텍스트로 된 제목에 충분한 여백을 주세요.** 내비게이션 바에 여러 개의 텍스트 버튼이 들어가게 되면, 버튼들의 글자들이 겹쳐, 구별할 수 없게 될 수도 있습니다. 버튼들 사이에 정해진 여백을 추가하여 간격을 유지하세요. 개발자 가이드는 여기에서 확인할 수 있습니다.



**Consider using a segmented control in a navigation bar to flatten your app's information hierarchy.** If you use a segmented control in a navigation bar, do so only at the top level of your hierarchy and be sure to choose accurate back-button titles at lower levels. For additional guidance, see [Segmented Controls](https://developer.apple.com/design/human-interface-guidelines/ios/controls/segmented-controls/).

> 앱의 정보를 풍성하게 하기 위해서 내비게이션 바에 segmented control 사용을 고려하세요. 내비게이션 바에segmented control을 사용한다면, 계층적인 구조의 가장 상위에서만 사용하고 낮은 단계에서는 뒤로 가기 버튼의 정확한 제목을 사용하세요. 더 많은 정보는 여기에서 확인할 수 있습니다.



<img width="303" alt="스크린샷 2020-02-19 오전 9 39 40" src="https://user-images.githubusercontent.com/40762111/74790716-cc88ae80-52fb-11ea-99d4-6e5090444322.png">