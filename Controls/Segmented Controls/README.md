# Segmented Controls
A segmented control is a linear set of two or more segments, each of which functions as a mutually exclusive button. Within the control, all segments are equal in width. Like buttons, segments can contain text or images. Segmented controls are often used to display different views. In Maps, for example, a segmented control lets you switch between Map, Transit, and Satellite views.

> Segmented control은 두 개 또는 그 이상의 segments의 선형적인 집합이며, 각 segment는 상호 배타적인 버튼 역할을 합니다. Control 내에서, 모든 segments는 동일한 폭을 가집니다. 버튼과 비슷하게, segments는 텍스트나 이미지를 가질 수 있습니다. Segmented controls는 종종 다른 뷰를 보여주기 위해서 사용됩니다. 예를 들어, 지도 앱에서, segmented control는 지도, 대중교통 및 위성 뷰로 변경하도록 도와줍니다.



<img width="273" alt="스크린샷 2020-04-13 오후 3 01 02" src="https://user-images.githubusercontent.com/40762111/79096298-b2b59600-7d97-11ea-935a-184aaf1ef93b.png">

**Limit the number of segments to improve usability.** Wider segments are easier to tap. On iPhone, a segmented control should have five or fewer segments.

> **사용성을 향상시키기 위해서 segements의 개수를 제한하세요.** segments의 폭이 더 넓으면 탭 하기 더 쉽습니다. 아이폰에서, segmented control은 5개 혹은 그 이하의 segments를 가져야 합니다.



**Try to keep segment content size consistent.** Because all segments have equal width, it doesn’t look great if content fills some segments but not others.

> **segment 콘텐츠 크기를 동일하게 유지하도록 하세요.** 모든 segments는 동일한 폭을 가지기 때문에, 몇몇의 segments만 콘텐츠가 채워지고 나머지는 그렇지 않다면 좋아 보지 않습니다.



**Avoid mixing text and images in a segmented control.** Although individual segments can contain text or images, mixing the two in a single control can lead to a disconnected and confusing interface.

> **Segmented control 내에서 텍스트와 이미지의 혼용은 피하세요.** 각각의 segments가 텍스트나 이미지를 포함할 수 있지만, 하나의 control에 두 가지를 섞는 것은 연결되지 않거나 혼란스러운 인터페이스가 될 수 있습니다.



**Position content appropriately in a custom segmented control.** If you change the background appearance of a segmented control, make sure content still looks good and doesn’t appear misaligned.

> **커스텀 segmented control에서 콘텐츠를 적절하게 배치하세요.** segmented control의 배경을 변경한다면, 콘텐츠가 잘 보이도록 유지하고, 정렬이 안된 것처럼 보이지 않도록 유의하세요.



For developer guidance, see [UISegmentedControl](https://developer.apple.com/documentation/uikit/uisegmentedcontrol).

> UISegmentedControl과 관련된 내용은 다음 문서를 참조하세요.