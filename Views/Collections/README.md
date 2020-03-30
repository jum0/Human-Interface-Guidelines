# Collections

A collection manages an ordered set of content, such as a set of photos, and presents it in a customizable and highly visual layout. Because a collection doesn’t enforce a strictly linear format, it’s particularly well-suited to displaying items that vary in size. Generally speaking, collections are ideal for showing off image-based content. Backgrounds and other decorative views can optionally be implemented to visually distinguish subsets of items.

> Collection은 사진 모음과 같이 순서가 있는 콘텐츠의 모음을 관리하고, 사용자가 직접 제작할 수 있는 시각적인 레이아웃으로 나타냅니다. Collection은 엄격하게 선형의 형식을 강요하지 않기 때문에, 특히 크기가 다양한 아이템들을 보여주는 것에 잘 어울립니다. 일반적으로, collection은 이미지에 기반한 콘텐츠를 돋보이게 하는데 이상적입니다. 배경과 기타 꾸며주는 뷰는 아이템의 하위 항목을 시각적으로 구별하기 위해서 선택적으로 구현될 수 있습니다.

<img width="274" alt="스크린샷 2020-03-30 오후 4 59 44" src="https://user-images.githubusercontent.com/40762111/77888914-f0022a00-72a7-11ea-92e9-28cee7a6b509.png">

Collections support both interactivity and animation. By default, you can tap to select, touch and hold to edit, and swipe to scroll. If your app requires it, more gestures can be added for performing custom actions. Within a collection, animations can be enabled whenever items are inserted, deleted, or reordered, and custom animations are also supported.

> Collections는 인터랙션과 애니메이션 모두 지원합니다. 기본적으로, 선택하기 위해서 탭하고, 편집하기 위해서 터치하며 잡고, 스크롤 하기 위해서 스와이프 할 수 있습니다. 앱에서 필요로 한다면, 커스텀 동작들을 수행하기 위해서 더 많은 제스처를 추가할 수 있습니다. Collection 내에서, 아이템들이 추가되거나, 삭제 혹은 재정렬될 때마다 애니메이션이 실행될 수 있고, 커스텀 애니메이션 또 한 지원됩니다.



**Avoid creating radical new designs when a standard row or grid layout is sufficient.** A collection should enhance the user experience, not become the center of attention. Make it easy to select an item. If it’s hard to tap an item in your collection, people will get frustrated and lose interest before reaching the content they want. Use adequate padding around content to keep the layout clean and prevent overlapping of content.

> **기본적인 행과 그리드 레이아웃으로 충분할 때, 지나치게 새로운 디자인 만드는 것을 피하세요.** Colletion은 사용자 경험을 향상시켜야 하지만, 주의를 집중시키는 것은 아닙니다. 아이템을 쉽게 선택할 수 있도록 하세요. Collection에서 아이템을 탭 하기 어렵다면, 사용자들은 그들이 원하는 콘텐츠에 접근하기 전에 흥미를 잃고 혼란스러워할 것입니다. 레이아웃을 깔끔하게 유지하기 위해서 콘텐츠를 둘러싸는 적당한 여백을 사용하고, 콘텐츠가 서로 겹치는 것을 피하세요.



**Consider using a table instead of a collection for text.** It’s generally simpler and more efficient to view and digest textual information when it’s displayed in a scrollable list.

> **텍스트는 collection보다 표를 사용하세요.** 스크롤 할 수 있는 리스트가 보일 때, 일반적으로 텍스트로 된 정보를 보여주고 이해시키는데 더 간단하며 효율적입니다.



**Use caution when making dynamic layout changes.** The layout of a collection can be changed at any time. If you dynamically change the layout while people are viewing and interacting with it, be sure the change makes sense and is easy to track. Unmotivated layout changes can make your app seem unpredictable and difficult to use. If context is lost due to a layout change, people are likely to feel like they’re no longer in control.

> **동적인 레이아웃을 변경할 때는 주의하세요.** Collection의 레이아웃은 언제든 변경될 수 있습니다. 사용자가 레이아웃에서 보고 인터랙션 중일 때 동적으로 레이아웃을 변경하면, 그 변화가 이해가 되고 쉽게 내용을 따라갈 수 있도록 주의하세요. 앱 내에서 이유가 없는 레이아웃의 변경은 예측할 수 없고 사용하기 어렵게 만듭니다. 레이아웃의 변경으로 컨텍스트가 상실된다면, 사용자는 더 이상 통제할 수 없다고 느낄 것입니다.



For developer guidance, see [UICollectionView](https://developer.apple.com/documentation/uikit/uicollectionview).

> 개발자 가이드는 다음 문서를 확인하세요.