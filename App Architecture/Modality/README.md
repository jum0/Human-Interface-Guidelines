# Modality
Modality is a design technique that presents content in a temporary mode that’s separate from the user's previous current context and requires an explicit action to exit. Presenting content modally can:

>  모달리티(Modality)는 사용자의 과거 현재 컨텍스트로부터 분리하여 임시로 콘텐츠를 나타내는 설계 기술이며, 종료하려면 명시적인 작업이 필요합니다. 콘텐츠를 모달로(modally) 나타내는 것을 다음과 같은 것을 할 수 있습니다.

- Help people focus on a self-contained task or set of closely related options

  > 사용자가 자체 지원 태스크나 밀접하게 관련된 옵션들을 집중할 수 있도록 도와줍니다.

- Ensure that people receive and, if necessary, act on critical information

  > 사용자가 중요한 정보를 수신하고 필요한 경우, 행동하는 것을 보장합니다.

![](https://user-images.githubusercontent.com/40762111/61592233-82c3d280-ac0b-11e9-977b-dd52edc02031.png)

iOS provides Alerts, Activity Views (or Share sheets), and Action Sheets that you use in specific situations in your app. To present custom modal content in your app, iOS 13 and later supports the following presentation styles.

> iOS는 애플리케이션의 특정 상황에서 Alerts, Activity Views (또는 Share sheets), 그리고 Action Sheets를 제공합니다. 애플리케이션에 커스텀 모달 콘텐츠를 표시하기 위해서, iOS 13 이상에서는 다음과 같은 프로젠테이션 스타일을 지원합니다.

## Sheet

The sheet presentation style appears as a *card* that partially covers the underlying content and dims all uncovered areas to prevent interaction with them. The top edge of the parent view or a previous card is visible behind the current card to help people remember the task they suspended when they opened the card. People dismiss a card by:

> sheet presentation 스타일은 기본 내용을 부분적으로 커버하고, 모든 미공개 영역과 상호작용 하는 것을 방지하기 위해서 어둡게 처리된 카드로 나타납니다. 부모 뷰의 상단 가장자리 또는 이전의 카드는 현재 카드(창)의 뒤에 보이는데, 이는 사용자들로 하여금 그들이 카드를 열었을 때, 중간에 멈추었던 작업들을 기억할 수 있도록 도와줍니다. 사람들은 다음과 같은 방법으로 카드를 폐기합니다.

- Swiping down from the top of the screen

> 화면의 상단에서 아래로 스와이프하기

- Swiping down from anywhere on the screen when card content is scrolled to the top

> 카드 콘텐츠가 맨 위로 스크롤될 때, 화면의 아무 곳에서나 아래로 스와이프 하기

- Tapping a button

> 버튼 탭하기

❗️Use a sheet for nonimmersive modal content that doesn't enable a complex task.

> 복잡한 작업을 하지 않도록 하는 (컴퓨터 시스템이 사용자를) 에워싸지 않는 듯한 모달 콘텐츠에 sheet를 사용하세요.



## Fullscreen

 The fullscreen presentation style covers the entire screen. The previous view is completely covered, minimizing visual distraction. People dismiss a full-screen modal view by tapping a button.

> ful lscreen presentation 스타일은 전체 화면을 커버합니다. 이전의 뷰는 완전히 커버되어 있고, 시각적으로 방해하는 것을 최소화합니다. 사용자는 버튼을 탭함으로써 full-screen 모달 뷰를 무시합니다.



Use a full-screen modal view for immersive content—such as videos, photos, or camera views—or a complex task that benefits from a full-screen presentation, such as marking up a document or editing a photo.

> 문서에 표시하거나 사진을 편집하는 등 full-screen presentation으로부터 도움을 받을 수 있는 복잡한 작업을 포함하여 비디오, 사진 또는 카메라 뷰 등 (컴퓨터 시스템이 사용자를) 에워싸는 콘텐츠에 full-screen 모달 뷰를 사용하세요.

```swift
NOTE
If you use the current context modal view style to display modal content within a split view pane, 
popover, or other view that isn’t fullscreen, you should switch to using a sheet when presenting 
modal content in a compact environment.

/*
current context 모달 뷰 스타일을 사용하여 분할 보기 창, 팝업 또는 전체 화면이 아닌 다른 보기 내에서 모달 콘텐츠를 보여주고 있는 경우,
컴팩트한 환경에서 모달 콘텐츠를 표기할 때 sheet를 사용하는 것으로 바꿔야 합니다.
*/
```

**Use modality when it makes sense.** Create a modal experience only when it’s critical to focus people’s attention on making a choice or performing a task that’s different from their current task. A modal experience takes people out of their current context and requires an action to dismiss, so it’s essential to use it only when it provides a clear benefit.

> **이해가 될 때 모달을 사용하세요.** 현재의 작업과 다른 작업을 수행하거나 선택하여 사용자의 주의를 집중시키는 것이 중요한 경우에만 모달 경험을 생성하세요. 모달 경험은 사용자에게 현재 상황을 벗어나고 무시하는 행동을 요구하므로, 모달이 명확한 유익을 제공하는 경우에만 사용해야 합니다.



**Reserve alerts for delivering essential—and ideally actionable—information.** Typically, an alert appears because something has gone wrong. Because an alert interrupts the experience and requires a tap to dismiss, it’s important for people to feel that the intrusion is warranted. For guidance, see Alerts.

> **필수적이고 이상적으로 실행 가능한 정보를 전달하기 위해서 알림을 예약하세요.** 일반적으로, 알림은 무엇인가가 잘못되었기 때문에 나타납니다. 알림은 경험을 방해하고 사용자에게 무시하기 위한 탭하기를 요구하기 때문에 사용자가 방해(intrusion)가 정당하다고 느끼도록 하는 것이 중요합니다. 자세한 내용은 Alerts를 참조하세요. (Views - Alerts)



**Keep modal tasks simple, short, and narrowly focused.** Avoid creating an app within your app. If a modal task is too complex, people can lose sight of the task they suspended when they entered the modal context. Be especially wary of creating modal tasks that involve a hierarchy of views because people can get lost and forget how to retrace their steps. If a modal task must contain subviews, provide a single path through the hierarchy and a clear path to completion. Avoid using a Done button for anything other than completing the task.

> **모달 작업은 간단하고, 짧게 그리고 가까스로(narrowly) 집중되도록 하세요.** 애플리케이션 내에서 애플리케이션 만드는 것을 피하세요. 모달 작업이 너무 복잡하면, 사용자들은 모달 상황(context)을 마주할 때, 기존의 하고 있던 작업의 집중이 흐트러질 수 있습니다. 특히 뷰의 계층이 포함되어 있는 모달 작업을 생성할 때 주의하세요. 왜냐하면 사용자는 되돌아가는 방법을 잃거나 잊어버릴 수 있습니다. 모달 작업이 반드시 하위 뷰를 포함해야한다면, 계층을 통해서 single path(현재 사용자가 어디에 있는지 알 수 있도록 표시한 path)와 완료하기까지의 명확한 path를 제공하세요. 작업을 완료하는 것 외에는 완료(Done) 버튼을 제공하지 마세요.



**Always include a button that dismisses the modal view.** For example, you might use Done or Cancel. Including a button ensures that the modal view is accessible to assistive technologies and provides an alternative to dismissal gestures.

> **모달 뷰를 끝내는 버튼을 항상 포함하세요.** 예를 들어, Done 또는 Cancel 버튼을 사용합니다. 버튼을 포함하는 것은 모달 뷰가 보조의 기술에 접근 가능할 수 있도록 도와주고, 그만두는 행동에 대안을 제공합니다.



**When necessary, help people avoid data loss by getting confirmation before closing a modal view.** Regardless of whether people use a dismiss gesture or a button to close the view, if the action could result in the loss of user-generated content, present an action sheet that explains the situation and gives people ways to resolve it.

> **필요하다면, 모달 뷰를 닫기 전에 사용자에게 동의를 구함으로써 데이터가 손실되는 것을 도와주세요.** 사용자가 그만두는 제스처를 취하거나 뷰를 닫는 버튼을 사용하여 사용자의 데이터가 손실되는 결과를 발생할 수 있다면, 사용자에게 상황을 설명하고 해결하는 방법을 알려주는 action sheet를 나타내세요.



**Don’t display a card that appears on top of a popover.** Although you can display a card within a popover, nothing should appear on top of a popover (except possibly an alert). In rare cases when you need to present a card after people take an action in a popover, close the popover before displaying the card.

> **Popover의 맨 위에 나타나는 카드는 보여주지 마세요.** popover 안에 카드를 보여줄 수 있지만, popover의 맨 위에는 아무것도 보여서는 안됩니다. (어쩌면 알림을 제외하고요). 드문 경우로 사용자가 popover에서 행동을 취한 후 카드를 보여줘야 할 때, 카드를 보여주기 전에 popover를 닫으세요.



**In general, display a title that identifies the modal task.** When people enter a modal task, they switch away from their previous context, so it’s a good idea to make the new context clear. You might also provide text in other parts of the view that more fully describes the task or provides guidance.

> **일반적으로, 모달에서 진행되는 일을 확인할 수 있는 제목을 보여주세요.** 사용자가 모달에서 제공되는 태스크를 시작하게 되는 경우, 사용자들은 그들이 이전에 진행하고 있던 환경과 달라지는 경험을 하게 됩니다. 따라서 새로운 환경이라는 점을 명확하게 알려주는 것이 좋습니다. 또한 뷰의 다른 부분에서 태스크에 대한 자세한 설명이나 가이드라인을 텍스트로 제공할 수 있습니다.

**Coordinate the modal view appearance with your app.** For example, when a modal view includes a navigation bar, it should use the same appearance as the navigation bar in your app.

> **모달 뷰의 디자인을 앱에 맞게 조정하세요.** 예를 들어서, 모달 뷰가 내비게이션 바를 포함할 때, 앱에서도 내비게이션 바와 같은 디자인을 사용해야 합니다.

 

**Choose a modal transition style that makes sense in your app.** Use a transition style that coordinates with your app and enhances the awareness of the temporary context shift. The default transition vertically slides the modal view up from the bottom of the screen and back down when it’s dismissed. Use consistent modal transition styles throughout your app.

> **앱에서 이해할 수 있는 모달 변경 스타일을 선택하세요.** 앱에 맞는 화면 변경 스타일을 사용하고, 일시적인으로 환경이 변화해도 사용자가 인지할 수 있도록 도와주세요. 모달의 기본적인 스타일은 모달이 화면의 아래에서 위 수직 방향으로 슬라이드 되고, 취소되었을 때 다시 돌아가는 것입니다. 앱 전체적으로 일관된 모달 화면 변경 스타일을 사용하세요.