# Page Controls
A page control shows the position of the current page in a flat list of pages. It appears as a series of small indicator dots, representing the available pages in the order they were opened. A solid dot denotes the current page. Visually, these dots are always equidistant, and are clipped if too many appear onscreen. Users can tap the leading or trailing edge of a page control to visit the next or previous page, but they can't tap a specific dot to go to a specific page. Navigation always occurs sequentially, usually by swiping the page to one side.

> Page Control은 페이지 목록에서 현재 페이지의 위치를 보여줍니다. Page Control은 작게 표시된 점들의 연속으로, 열리는 순서에 있는 이용 가능한 페이지를 나타내는 것으로 보입니다. 속이 찬 점은 현재 페이지를 의미합니다. 시각적으로, 이런 점들은 항상 같은 간격으로 있으며, 화면에 나타나는 것들이 너무 많다면 잘립니다. 사용자들은 페이지의 leading과 trailing 끝부분을 탭 하여 다음 페이지나 이전 페이지로 이동할 수 있지만, 특정 점을 탭 하여 특정 페이지로 이동할 수는 없습니다. 내비게이션은 항상 순차적으로 발생하고, 보통 페이지를 한 쪽 방향으로 스와이프 합니다.

<img width="268" alt="스크린샷 2020-04-02 오후 7 59 44" src="https://user-images.githubusercontent.com/40762111/78242233-99e9ec80-751c-11ea-9998-1fc29ee72742.png">

**Don’t use a page control with hierarchical pages.** A page control doesn’t show how pages are related or indicate which page corresponds to each dot. This type of control is designed for pages that are peers to one another.

> **계층적인 구조에서는 page control을 사용하지 마세요.** Page control은 각각의 점에 어떤 페이지가 응답하여 얼마나 많은 페이지와 관련이 있는지 혹은  나타내는지 보여주지 않습니다. 이런 control의 타입은 서로가 같은 계층으로 설계됩니다.



**Don’t display too many pages.** More than about 10 dots are hard to count at a glance, and more than about 20 open pages are time-consuming to visit in sequence. If your app needs to display more than 20 pages as peers, consider using a different arrangement—such as a grid—that enables nonsequential navigation.

> **너무 많은 페이지를 보여주지 마세요.** 10개가 넘어가는 점들은 한눈에 세기 어렵고, 20개의 페이지보다 많으면 순서대로 이동하는데 시간이 낭비됩니다. 같은 계층으로 20개가 넘는 페이지를 보여주는 것이 필요하다면, 그리드와 같이 순차적인 내비게이션이 필요하지 않는 다른 구성 사용하는 것을 고려하세요.



**Center page controls at the bottom of the screen.** A page control should always be centered and positioned between the bottom of the content and the bottom of the screen. This keeps it visible, without blocking content.

> **Page controls을 화면 하단에 가운데에 정렬하세요.** Page control은 항상 가운데 정렬되어야 하며, 화면의 하단과 콘텐츠의 아래 사이에 위치해야 합니다. 이러한 배치는 콘텐츠를 가리지 않으며 보이도록 유지합니다.



For developer guidance, see [UIPageControl](https://developer.apple.com/documentation/uikit/uipagecontrol).

> 개발자 가이드는 다음 문서를 확인하세요.