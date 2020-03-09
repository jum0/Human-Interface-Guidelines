# Action Sheets

An action sheet is a specific style of alert that appears in response to a control or action, and presents a set of two or more choices related to the current context. Use an action sheet to let people initiate tasks, or to request confirmation before performing a potentially destructive operation. On smaller screens, an action sheet slides up from the bottom of the screen. On larger screens, an action sheet appears all at once as a popover.

> Action sheet는 control이나 action에 응답하여 나타나는 alert의 세부 style이고, 현재 컨텍스트와 관련된 2개 또는 그 이상의 선택지를 제공합니다. 사용자가 tasks를 초기화하거나, 잠재적으로 삭제하는 작업을 수행하기 이전에 확인을 요청할 때 action sheet를 사용하세요. 작은 화면에서 action sheet는 화면의 하단에서 올라옵니다. 큰 화면에서는 popover로 한꺼번에 나타납니다.

<img width="268" alt="스크린샷 2020-03-09 오후 6 55 24" src="https://user-images.githubusercontent.com/40762111/76202066-9b830600-6237-11ea-9a23-48ad3aeca004.png">

**Provide a Cancel button if it adds clarity.** A Cancel button instills confidence when the user is abandoning a task. Cancel buttons should always be included in action sheets at the bottom of the screen.

> **Cancel 버튼이 명확하게 추가되면 제공하세요.** Cancel 버튼은 사용자가 작업을 그만둘 때, 사용자가 신뢰할 수 있는 느낌을 줍니다. Cancel 버튼은 항상 action sheet에서 화면의 하단에 포함되어야 합니다.



**Make destructive choices prominent.** Use red for buttons that perform destructive or dangerous actions, and display these buttons at the top of an action sheet.

> **삭제하는 선택지는 눈에 띄게 만드세요.** 삭제하거나 위험한 작업을 수행할 때 빨간색의 버튼을 사용하고 이러한 버튼들이 action sheet의 최상단에 보여주세요.



**Avoid enabling scrolling in an action sheet.** If an action sheet has too many options, people must scroll to see all of the choices. Scrolling requires extra time to make a choice and is hard to do without inadvertently tapping a button.

> **Action sheet가 scrolling 되는 것을 피하세요.** Action sheet에 너무 많은 선택지가 있다면, 사용자는 전체를 확인하기 위해서 scroll 해야만 합니다. Scrolling 하는 것은 선택을 하는데 약간의 시간을 더 필요로 하고, 실수로 버튼을 tap 하지 않고는 하기 어렵습니다.

For developer guidance, see the [UIAlertControllerStyleActionSheet](https://developer.apple.com/documentation/uikit/uialertcontrollerstyle/uialertcontrollerstyleactionsheet) constant in [UIAlertController](https://developer.apple.com/documentation/uikit/uialertcontroller).

> 개발자 가이드는 다음 문서를 확인하세요.