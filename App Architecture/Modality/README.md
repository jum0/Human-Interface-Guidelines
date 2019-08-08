# Modality
Modality is a design technique that presents content in a temporary mode that’s separate from the user's previous current context and requires an explicit action to exit. Presenting content modally can:

*모달리티(Modality)는 사용자의 과거 현재 컨텍스트로부터 분리해서 임시로 콘텐츠를 표시하는 설계 기술이며, 종료하려면 명시적인 작업이 필요합니다. 콘텐츠를 모달로(modally) 나타내는 것을 다음과 같은 것을 할 수 있습니다.*

- Help people focus on a self-contained task or set of closely related options

  *사용자가 자체 지원 태스크나 밀접하게 관련된 옵션들을 집중할 수 있도록 도와줍니다.*

- Ensure that people receive and, if necessary, act on critical information

  *사용자가 중요한 정보를 수신하고 필요한 경우, 행동하는 것을 보장합니다.*

![](https://user-images.githubusercontent.com/40762111/61592233-82c3d280-ac0b-11e9-977b-dd52edc02031.png)

iOS provides Alerts, Activity Views (or Share sheets), and Action Sheets that you use in specific situations in your app. To present custom modal content in your app, iOS 13 and later supports the following presentation styles.

*iOS는 애플리케이션의 특정 상황에서 Alerts, Activity Views (또는 Share sheets), 그리고 Action Sheets를 제공합니다. 애플리케이션에 커스텀 모달 콘텐츠를 표시하기 위해서, iOS 13 이상에서는 다음과 같은 프로젠테이션 스타일을 지원합니다.*

## Sheet

The sheet presentation style appears as a *card* that partially covers the underlying content and dims all uncovered areas to prevent interaction with them. The top edge of the parent view or a previous card is visible behind the current card to help people remember the task they suspended when they opened the card. People dismiss a card by:

*sheet presentation 스타일은 기본 내용을 부분적으로 커버하고, 모든 미공개 영역과 상호작용 하는 것을 방지하기 위해서 어둡게 처리된 카드로 나타납니다. 부모 뷰의 상단 가장자리 또는 이전의 카드는 현재 카드(창)의 뒤에 보이는데, 이는 사용자들로 하여금 그들이 카드를 열었을 때, 중간에 멈추었던 작업들을 기억할 수 있도록 도와줍니다. 사람들은 다음과 같은 방법으로 카드를 폐기합니다.*

- Swiping down from the top of the screen

*화면의 상단에서 아래로 스와이프하기*

- Swiping down from anywhere on the screen when card content is scrolled to the top

*카드 콘텐츠가 맨 위로 스크롤될 때, 화면의 아무 곳에서나 아래로 스와이프 하기*

- Tapping a button

*버튼 탭하기*

❗️Use a sheet for nonimmersive modal content that doesn't enable a complex task.

*복잡한 작업을 하지 않도록 하는 (컴퓨터 시스템이 사용자를) 에워싸지 않는 듯한 모달 콘텐츠에 sheet를 사용하세요.*



## Fullscreen

 The fullscreen presentation style covers the entire screen. The previous view is completely covered, minimizing visual distraction. People dismiss a full-screen modal view by tapping a button.

*ful lscreen presentation 스타일은 전체 화면을 커버합니다. 이전의 뷰는 완전히 커버되어 있고, 시각적으로 방해하는 것을 최소화합니다. 사용자는 버튼을 탭함으로써 full-screen 모달 뷰를 무시합니다.*



Use a full-screen modal view for immersive content—such as videos, photos, or camera views—or a complex task that benefits from a full-screen presentation, such as marking up a document or editing a photo.

*문서에 표시하거나 사진을 편집하는 등 full-screen presentation으로부터 도움을 받을 수 있는 복잡한 작업을 포함하여 비디오, 사진 또는 카메라 뷰 등 (컴퓨터 시스템이 사용자를) 에워싸는 콘텐츠에 full-screen 모달 뷰를 사용하세요.*

```
NOTE
If you use the current context modal view style to display modal content within a split view pane, popover, or other view that isn’t fullscreen, you should switch to using a sheet when presenting modal content in a compact environment.

current context 모달 뷰 스타일을 사용하여 분할 보기 창, 팝업 또는 전체 화면이 아닌 다른 보기 내에서 모달 콘텐츠를 보여주고 있는 경우, 컴팩트한 환경에서 모달 콘텐츠를 표기할 때 sheet를 사용하는 것으로 바꿔야 합니다.
```









