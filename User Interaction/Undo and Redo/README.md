# Undo and Redo
Many apps allow people to shake the device to undo and redo certain operations, such as typing or deleting. When initiated in this manner, an alert asks the user to confirm or cancel the undo or redo operation.

> 많은 앱들은 사용자가 글씨를 쓰거나 지우는 것 등 특정한 작업들을 undo(실행 취소) 나 redo(재실행) 하기 위해서 디바이스 흔드는 것을 허용합니다. 이러한 방식으로 시작되면, 사용자에게 undo 또는 redo 작업을 확인하거나 취소할 것을 요청하는 알림이 표시됩니다.



<img width="285" alt="스크린샷 2020-02-28 오전 11 58 54" src="https://user-images.githubusercontent.com/40762111/75506582-cabc9a80-5a21-11ea-9009-02d6edc7523e.png">

**Briefly and precisely describe the operation to be undone or redone.** The undo and redo alert title automatically includes a prefix of “Undo ” or “Redo ” (including the trailing space). You need to provide an additional word or two that describe what’s being undone or redone, to appear after this prefix. For example, you might create alert titles such as “Undo Name” or “Redo Address Change.”

> **실행이 취소되고 재실행하는 작업을 간략하고 정확하게 설명해 주세요.** 실행 취소나 재실행 알림 제목은 당연하게 "Undo"나 "Redo"로 시작하게 됩니다.(그 뒤로 공백을 포함합니다). 추가적으로 이 접두사 뒤에 실행 취소나 재실행 중인 내용을 설명하는 단어를 제공해야 합니다. 예를 들어, "Undo Name(이름 실행 취소)" 또는 "Redo Address Change(주소 변경 재실행)"과 같은 알림 제목을 만들 수 있습니다.



**If you use the shake gesture for undo and redo, don’t use it for other actions.** Although you can programmatically give multiple meanings to the shake gesture, you run the risk of confusing people and making your app unpredictable.

> **실행을 취소하거나 다시 실행하기 위해서 흔드는 제스처를 사용하면, 다른 행동은 사용하지 마세요.** 흔드는 제스처에 프로그래밍적으로 다양한 의미를 부여할 수 있지만, 사용자들이 혼란스러워하거나 앱을 복잡하게 만듭니다.



**Provide undo and redo buttons sparingly.** It’s confusing when apps provide multiple ways to perform the same task. If your app truly warrants dedicated undo and redo buttons, use the standard system-provided icons and put them in an expected location, such as a navigation bar.

> **실행 취소와 다시 실행 버튼은 조금만 제공하세요.** 앱에서 같은 작업을 수행하기 위해 여러 선택지를 제공하면 혼란스럽습니다. 앱에서 실행 취소 및 다시 실행 버튼을 사용할 수 있는 경우, 내비게이션 바와 같이 사용자들이 예상 가능한 위치에 시스템에서 기본으로 제공하는 아이콘을 사용하세요.



**Perform undo and redo operations in the current context only.** Undo and redo should have a clear and immediate effect on the current context, not an earlier one.

> **현재 컨텍스트(환경)에서만 실행 취소 및 다시 실행 작업을 수행하세요.** 실행 취소와 다시 실행은 이전 컨텍스트가 아닌 현재 컨텍스트에서 명확하고 즉각적인 영향을 주어야 합니다.



For developer guidance, see [UndoManager](https://developer.apple.com/documentation/foundation/undomanager).

> 개발자 가이드는 다음 문서를 확인하세요.