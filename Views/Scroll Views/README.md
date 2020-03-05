# Scroll Views

A scroll view allows users to browse content, such as text in a document or a collection of images, that’s larger than the visible area. As people swipe, flick, drag, tap, and pinch, a scroll view follows the gesture, revealing or zooming content in a way that feels natural. A scroll view itself has no appearance, but does display transient scrolling indicators as people interact with it. A scroll view can also be configured to operate in paging mode, where scrolling reveals an entirely new page of content rather than moving around the current page.

> Scroll view는 사용자가 문서의 텍스트나 이미지 모음과 같이 볼 수 있는 영역보다 큰 콘텐츠를 둘러볼 수 있도록 합니다. 사용자가 swipe, flick, drag, pinch를 함으로써 scroll view는 자엽스럽게 콘텐츠를 드러내거나 zoom 하며 제스처를 따라갑니다. Scroll view는 그 자체로 나타나지 않지만, 사용자들이 상호작용하는 것처럼 잠깐 동안 scrolling 할 때의 직사각형 네모(indicators)를 보여줍니다.  Scroll view는 또한 페이징 모드에서 작동하도록 구성될 수 있는데, 여기서 스크롤 하면 현재 페이지를 이동하지 않고 완전히 새로운 콘텐츠 페이지가 나타나게 됩니다.

<img width="277" alt="스크린샷 2020-03-05 오후 10 50 45" src="https://user-images.githubusercontent.com/40762111/75987771-d33a3700-5f33-11ea-8749-bebba7e6eb55.png">

**Support zoom behavior appropriately.** If it makes sense in your app, let people pinch or double-tap to zoom in and out. When you enable zoom, set maximum and minimum scale values that make sense. For example, zooming in on text until a single character fills the screen probably doesn’t make sense in most apps.

> **적절하게 zoom 행동을 지원하세요.** 앱에서 의미가 통한다면, 사용자가 zoom in과 out을 하기 위해서 pinch나 double-tap을 하도록 하세요. zoom을 사용할 수 있도록 할 때, 이해하기 쉬운 최댓값과 최솟값을 설정하세요. 예를 들어, 대부분의 앱에서 zoom in을 통해서 하나의 문자가 화면 전체를 차지하도록 하는 것은 어색할 수 있습니다. 



**Consider showing a page control element when a scroll view is in paging mode.** A page control shows how many pages, screens, or other chunks of content are available and indicates which one is currently visible. If you show a page control with a scroll view, disable the scrolling indicator on the same axis to avoid confusion. For additional guidance, see [Page Controls](https://developer.apple.com/design/human-interface-guidelines/ios/controls/page-controls/).

> **Scroll view가 paging mode에 있을 때, page control element 보여주는 것을 고려하세요.** Page control은 페이지와 화면들 또는 이용할 수 있는 콘텐츠의 양이 얼마나 되는지 보여주고, 어떤 부분이 현재 보이고 있는지 알려줍니다. Scroll view와 함께 page control을 보여준다면, 혼란을 피하기 위해 같은 선상에 scrolling indicator가 나타나지 않도록 하세요. 더 많은 내용은 다음 문서를 확인하세요.



**Don’t place a scroll view inside of another scroll view.** Doing so creates an unpredictable interface 
that’s difficult to control.

> **또 다른 scroll view 안에 scroll view을 배치하지 마세요.** 이렇게 하면 컨트롤하기 어려운 예측 불가능한 인터페이스가 만들어집니다.



**In general, display one scroll view at a time.** People often make large swipe gestures when scrolling, and it can be hard to avoid interacting with a neighboring scroll view on the same screen. If you need to put two scroll views on one screen, consider allowing them to scroll in different directions so one gesture is less likely to affect both views. For example, when an iPhone is in portrait orientation, the Stocks app shows stock quotes that scroll vertically above company-specific information that scrolls horizontally.

> **일반적으로 한 번에 하나의 scroll view를 보여주세요.** 사용자들은 종종 scrolling을 할 때 크게 swipe를 하는데, 이것은 같은 화면에서 이웃하고 있는 scroll view와 기능적으로 부딪힐 수 있습니다. 한 화면에 두 개의 scroll view를 넣고 싶다면, 두 view가 서로 다른 방향으로 scroll 되도록 하여, 하나의 gesture가 서로 다른 view에 최소한으로 영향을 미치도록 하세요. 예를 들어 아이폰이 세로 방향일 때, 주식 앱에서 세로 방향으로 scroll을 하면 주식 시세가 보이고, 가로 방향으로 scroll을 하면 기업의 정보가 나타납니다.



For developer guidance, see [UIScrollView](https://developer.apple.com/documentation/uikit/uiscrollview)

> 개발자 가이드는 다음 문서를 참조하세요.