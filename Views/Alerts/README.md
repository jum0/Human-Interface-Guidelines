# Alerts

Alerts convey important information related to the state of your app or the device, and often request feedback. An alert consists of a title, an optional message, one or more buttons, and optional text fields for gathering input. Aside from these configurable elements, the visual appearance of an alert is static and can’t be customized.

> Alerts는 앱이나 기기의 상태와 관련해 중요한 정보를 전달하고 종종 피드백을 요청합니다. Alert는 제목, 선택적인 메시지, 하나 이상의 버튼, 선택적인 입력을 받기 위한 text fields로 구성됩니다. 이러한 구성할 수 있는 요소를 제외하면 alert의 시각적인 형태는 고정적이고 사용자가 변경할 수 없습니다.

<img width="277" alt="스크린샷 2020-03-06 오후 3 08 18" src="https://user-images.githubusercontent.com/40762111/76057277-6028d300-5fbc-11ea-97ec-ad3d78282d8a.png">

**Minimize alerts.** Alerts disrupt the user experience and should only be used in important situations like confirming purchases and destructive actions (such as deletions), or notifying people about problems. The infrequency of alerts helps ensure that people take them seriously. Ensure that each alert offers critical information and useful choices.

> **Alerts를 최소화하세요.** Alerts는 사용자 경험을 방해하고, 오직 중요한 상황에서만 사용되어야 하는데, 구매를 확인하거나 삭제와 같이 제거하는 행동 또는 사용자에게 문제에 대해서 알려줄 때입니다. Alerts를 드물게 사용하는 것은 사용자가 alerts를 진지하게 생각하는 데 도움을 줍니다. 각각의 alert가 중요한 정보와 유용한 선택을 제공하도록 하세요.



**Test the appearance of alerts in both orientations.** An alert may appear differently in landscape mode and portrait mode. Optimize alert text so it reads well in any orientation without scrolling.

> **가로 방향과 세로 방향 무두에서 alerts의 형태를 테스트해보세요.** Alert가 가로 화면 모드와 세로 화면 모드에서 다르게 보일 수도 있습니다.  Alert의 최적화하여 모든 방향에서 scrolling 하지 않고 잘 읽을 수 있도록 하세요.



For developer guidance, see [UIAlertController](https://developer.apple.com/documentation/uikit/uialertcontroller).

> 개발자 가이드는 다음 문서를 확인하세요.



### Alert Titles and Messages

**Write short, descriptive, multiword alert titles.** The less text people have to read onscreen, the better. Try to craft a title that avoids adding extra text as a message. Because single-word titles rarely provide useful information, consider asking a question or using short sentences. Whenever possible, keep titles to a single line. If the title is a complete sentence, use sentence-style capitalization and appropriate ending punctuation. If the title is a sentence fragment, use title-style capitalization and don’t add ending punctuation.

> **간략하고 설명적인 단어로 된 alert 제목을 쓰세요.** 사용자가 화면에서 더 적은 텍스트를 읽을수록 더 좋습니다. 메시지로 추가적인 텍스트가 필요하지 않게, 제목을 만들어보세요. 하나의 단어로 된 제목은 유용한 정보를 제공하기 힘들기 때문에, 질문을 하거나 짧은 문장 사용하는 것을 고려하세요. 가능하다면, 제목을 한 줄로 유지하세요. 제목이 완전한 문장이라면, 문장 형식의 대문자를 사용하고 적절한 끝 문장 부호를 사용하세요. 제목이 나누어진 문장이라면, 제목 형식의 대문자를 사용하고 끝 문장 부호를 추가하지 마세요.



**If you must provide a message, write short, complete sentences.** Try to keep messages short enough to fit on one or two lines to prevent scrolling. Use sentence-style capitalization and appropriate punctuation.

> **메시지를 제공해야만 한다면, 짧고 완전한 문장을 사용하세요.** Scrolling을 하지 않도록 메시지를 한두 문장으로 유지하세요. 문장 형식의 대문자를 사용하고 적절한 문장 끝 부호를 사용하세요.



**Avoid sounding accusatory, judgmental, or insulting.** People know that alerts notify them about problems and dangerous situations. As long as you use a friendly tone, it’s better to be negative and direct than positive and oblique. Avoid pronouns such as you, your, me, and my, which are sometimes interpreted as insulting or patronizing.

> **비난하거나 비판적이며 모욕적으로 들리지 않도록 하세요.** 사용자는 alerts가 그들에게 문제와 위험한 상황에 대해서 알려주는 것을 알고 있습니다. 친근한 어조를 사용하는 한 긍정적이고 완곡한 것보다 부정적이며 직설적인 것이 더 좋습니다. 하지만, "너" 또는 "나"와 같이 상황에 따라 모욕적이거나 아랫사람 대하는 듯하게 느껴지는 것들은 피하세요.



**Avoid explaining the alert buttons.** If your alert text and button titles are clear, there should be no need to explain what the buttons do. In rare cases where you must provide guidance, use the word *tap*, preserve capitalization when referencing buttons, and don’t enclose button titles in quotes.

> **Alert 버튼은 설명하지 마세요.** Alert 텍스트와 버튼 제목이 명확하다면, 버튼의 역할에 대해서 설명하지 않아도 됩니다. 드물게 가이드를 제공해야만 하는 경우, *tap* 단어를 사용하고, 버튼을 참조할 때 대문자를 유지하며, 인용문에 버튼 제목을 넣지 마세요.



### Alert Buttons

**Generally, use two-button alerts.** Two-button alerts provide an easy choice between two alternatives. Single-button alerts inform, but give no control over the situation. Alerts with three or more buttons create complexity and can require scrolling, which is a bad user experience. If you find that you need more than two choices, consider using an action sheet instead. See [Action Sheets](https://developer.apple.com/design/human-interface-guidelines/ios/views/action-sheets/).

> **일반적으로, 두 개의 버튼을 가진 alerts를 사용하세요.** 두 개의 버튼을 가진 alerts는 쉽게 선택할 수 있는 두 가지 선택지를 제공합니다. 하나의 버튼을 가진 alerts는 정보를 주지만, 상황을 제어할 수는 없습니다. 세 개 이상의 버튼을 가진 alerts는 복잡하고 scrolling을 필요로 할 수 있는데, 이는 사용자에게 부정적인 경험을 줍니다. 두 개보다 많은 선택지가 필요하다면, 대신에 action sheet 사용하는 것을 고려하세요. Action Sheets에 관한 내용은 다음 문서를 확인하세요.



**Give alert buttons succinct, logical titles.** The best button titles consist of one or two words that describe the result of selecting the button. As with all button titles, use title-style capitalization and no ending punctuation. To the extent possible, use verbs and verb phrases that relate directly to the alert title and message—for example, View All, Reply, or Ignore. Use OK for simple acceptance. Avoid using Yes and No.

> **간단명료하고 논리적인 alert 버튼을 제공하세요.** 버튼을 선택했을 때의 결과를 설명해 주는 하나 또는 두 개의 단어로 구성된 버튼 제목이 가장 좋습니다. 모든 버튼 제목들은 제목 형식의 대문자를 사용하고, 문장 끝 부호를 사용하지 마세요. 가능한 한, alert 제목과 메시지에 직접 관련된 동사와 동사구를 사용하세요. 예를 들어, 모두 보기(View All), 응답하기(Reply), 무시하기(Igore) 등이 있습니다. OK는 간단한 수락에 적합합니다. Yes와 No를 사용하는 것은 피해주세요.



**Place buttons where people expect them.** In general, buttons people are most likely to tap should be on the right. Cancel buttons should always be on the left.

> **사용자들이 예측하는 곳에 버튼을 구성하세요.** 일반적으로, 대부분의 사용자들이 tap 하는 버튼은 오른쪽에 위치해야 합니다. 취소하기 버튼은 항상 왼쪽에 있어야 합니다.



**Label cancellation buttons appropriately.** A button that cancels an alert’s action should always be 

labeled Cancel.

> **취소 버튼은 적절하게 명명하세요.** Alerts의 행동을 취소하는 버튼은 항상 취소하기(Cancel)입니다.



**Identify destructive buttons.** If an alert button results in a destructive action, such as deleting content, set the button’s style to Destructive so that it gets appropriate formatting by the system. For developer guidance, see the [UIAlertActionStyleDestructive](https://developer.apple.com/documentation/uikit/uialertactionstyle/uialertactionstyledestructive) constant of [UIAlertAction](https://developer.apple.com/documentation/uikit/uialertaction). Additionally, provide a Cancel button so people can safely opt out of the destructive action. Make the Cancel button bold by marking it as the default button.

> **제거하는 버튼을 확인하세요.** Alert 버튼이 콘텐츠를 삭제하는 것과 같이 제거하는 행동을 취하게 된다면, 버튼의 스타일을 Destructive로 설정하여 시스템에 의해 적절하게 형식을 따르게 하세요. 개발자 가이드는 다음 문서를 확인하세요. 부가적으로, 사용자가 안전하게 제거하는 행동의 컨텍스트에서 나올 수 있도록 취소하기(Cancel) 버튼을 제공하세요. 취소하기(Cancel) 버튼을 기본 버튼으로 굵게 표시하세요.



**Allow people to cancel alerts by exiting to the Home screen.** Accessing the Home screen while an alert is visible exits the app. It should also produce the same effect as tapping the Cancel button—that is, the alert is dismissed without performing any action. If your alert doesn’t have a Cancel button, consider implementing a cancel action in your code that runs when someone exits your app.

> **사용자가 홈 화면으로 나감으로써 alerts를 취소할 수 있도록 하세요.** Alert가 보이는 동안 홈 화면에 접근하는 것은 앱을 나가는 것입니다. 그것 또한 취소하기(Cancel) 버튼을 tap 하는 것과 같은 효과를 줘야 합니다. 즉, 특별한 행동을 취하지 않고 alert는 무시됩니다. Alert에 취소하기(Cancel) 버튼이 없다면, 사용자가 앱을 나갈 때 실행되는 취소하는 행동을 코드에 추가하세요.