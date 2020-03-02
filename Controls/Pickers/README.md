# Pickers
A picker includes one or more scrollable lists of distinct values, each of which has a single selected value—appearing in darker text in the center of the view. A picker is often displayed at the bottom of the screen or in a popover when the user is editing a field or tapping a menu. Pickers can also appear inline, such as while editing a date in a Calendar event. The height of a picker is roughly the height of five rows of list values. The width of a picker is either the width of the screen or its enclosing view, depending on the device and context.

> Picker는 하나 이상의 스크롤 할 수 있는 고유한 값을 가지고 있는데, 각각은 화면의 중앙에 어두운 글자로 표시되는 하나의 선택된 값을 가지고 있습니다. Picker는 보통 사용자가 필드를 편집하거나 메뉴를 가볍게 터치할 때, 화면의 하단부나 팝업으로 표시됩니다. Picker는 또한 캘린더 앱의 이벤트에서 날짜를 편집할 때와 같이 내부에서 보일 수도 있습니다. Picker의 높이는 대략 다섯 개 값들의 높이입니다. 가로의 길이는 화면의 가로 길이이거나, 기기와 context에 따라서 enclosing view(?)입니다.

<img width="272" alt="스크린샷 2020-03-02 오후 6 22 01" src="https://user-images.githubusercontent.com/40762111/75662691-da064700-5cb2-11ea-8234-3db87e10e329.png">

> [See animation](https://developer.apple.com/design/human-interface-guidelines/ios/controls/pickers/)

**Use predictable and logically ordered values.** Many values in a picker may be hidden when the scrollable lists are stationary. It's best when people can predict what these values are, such as with a list of alphabetized countries, so they can move through the lists quickly.

> **예측할 수 있고 논리적으로 정렬된 값을 사용하세요.** 스크롤 할 수 있는 리스트가 고정되어 있을 때, picker에 있는 많은 값들은 아마 보이지 않을 겁니다. 사용자들이 알파벳순으로 정렬된 나라의 리스트와 같이, 이러한 값들이 무엇인지 예상할 수 있어서 리스트에서 빠르게 이동할 수 있다면, 가장 좋습니다. 



**Avoid switching screens to show a picker.** A picker works well when displayed in context, below or in close proximity to the field being edited.

> **Picker를 보여주기 위해 화면 변경하는 것을 피하세요.** Picker는 편집 중인 필드나 그 아래의 컨텍스트와 가깝게 표시될 때, 더욱 잘 기능을 합니다.



**Use a table instead of a picker for large value lists.** Long lists can be tedious to navigate in a picker. A table has adjustable height and can include an index, making scrolling much faster.

> **리스트의 값들이 많다면 picker 대신 table을 사용하세요.** 리스트가 길다면 picker에서 이동하는 게 귀찮을 수 있습니다. Table은 높이를 조정할 수 있고, 인덱스를 포함할 수 있어서 빠르게 스크롤 할 수 있습니다.



For developer guidance, see [UIPickerView](https://developer.apple.com/documentation/uikit/uipickerview).

> 개발자 가이드는 다음 문서를 확인하세요.



### Date Pickers

A date picker is an efficient interface for selecting a specific date, time, or both. It also provides an interface for displaying a countdown timer.

> Date picker는 구체적인 날짜와 시간 또는 둘 다 선택하는데 효과적인 인터페이스입니다. Date picker는 타이머를 보여주는 인터페이스도 제공합니다.

<img width="272" alt="스크린샷 2020-03-02 오후 6 21 35" src="https://user-images.githubusercontent.com/40762111/75662687-d7a3ed00-5cb2-11ea-849c-c48327f61307.png">

> [See animation](https://developer.apple.com/design/human-interface-guidelines/ios/controls/pickers/)



A date picker has four modes, each of which presents a different set of selectable values.

> Date picker는 네 가지 모드가 있는데, 각각의 모드는 다른 종류의 선택할 수 있는 값들을 제공합니다.



- **Date.** Displays months, days of the month, and years.

  > **날짜.** 연도, 월, 일을 보여줍니다. 

- **Time.** Displays hours, minutes, and (optionally) an AM/PM designation.

  > **시간.** 시간, 분, 그리고 (옵션으로) AM/PM을 지정해서 보여줍니다. 

- **Date and time.** Displays dates, hours, minutes, and (optionally) an AM/PM designation.

  > **날짜와 시간.** 날짜, 시간, 분, 그리고 (옵션으로) AM/PM을 지정해서 보여줍니다.

- **Countdown timer.** Displays hours and minutes, up to a maximum of 23 hours and 59 minutes.

  > **타이머.** 23시간 59분을 최대로 시간, 분을 보여줍니다.

  

The exact values shown in a date picker and their order depend upon the user’s locale.

> Date picker에서는 정확인 값을 보여주고 순서는 사용자의 환경에 따라 설정할 수 있습니다.



**Consider providing less granularity when specifying minutes.** By default, a minute list includes 60 values (0 to 59). You can optionally increase the minute interval as long as it divides evenly into 60. For example, you might want quarter-hour intervals (0, 15, 30, and 45).

> **분을 명시할 때는 입도를 최소화하여 제공하는 것을 고려하세요.** 기본적으로, 분 리스트는 60개의 값(0부터 59까지)을 가지고 있습니다.  분 간격을 일정하게 60개로 나누어, 선택적으로 증가시킬 수 있습니다. 예를 들어, 4분의 1시간 간격과 같이 말입니다.(0, 15, 30, 45)



For developer guidance, see [UIDatePicker](https://developer.apple.com/documentation/uikit/uidatepicker).

> 개발자 가이드는 다음 문서를 확인하세요.