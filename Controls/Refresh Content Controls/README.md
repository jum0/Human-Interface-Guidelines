# Refresh Content Controls
A refresh control is manually initiated to immediately reload content, typically in a table view, without waiting for the next automatic content update to occur. A refresh control is a specialized type of activity indicator, is hidden by default, and becomes visible when dragging down on the view to be reloaded. In Mail, for example, you can drag the list of Inbox messages down to check for new messages.

> Refresh control은 콘텐츠를 즉시 다시 로드하기 위해서 수동으로 시작되는데, 대표적으로 테이블 뷰에서 다음의 자동 콘텐츠 업데이트가 수행될 때까지 기다리지 않습니다. Refresh control은 activity indicator로 기본적으로는 숨겨져 있으며, 다시 로드하기 위해 뷰에서 아래로 드래그할 때, 볼 수 있게 됩니다. 예를 들어, 메일 앱에서 새로운 메시지를 확인하기 위해서 메시지 리스트를 드래그할 수 있습니다.

<img width="269" alt="스크린샷 2020-03-18 오전 11 55 24" src="https://user-images.githubusercontent.com/40762111/76920703-79604680-690f-11ea-86d4-f05fffe04d9d.png">

[Example](https://developer.apple.com/design/human-interface-guidelines/ios/controls/refresh-content-controls/)

**Perform automatic content updates.** Although people appreciate being able to trigger an immediate content refresh, they also expect automatic refreshes to occur periodically. Don’t make users responsible for initiating every update. Keep data fresh by updating it regularly.

> **자동 콘텐츠 업데이트를 수행하세요.** 사용자는 즉각적인 콘텐츠 업데이트를 실행할 수 있다는 점에 감사해하지만, 또한 주기적으로 업데이트가 자동으로 수행될 것을 기대합니다. 매번 업데이트를 사용자가 하도록 만들지 마세요. 정기적으로 데이터가 업데이트 되도록 유지하세요.



**Supply a short title only if it adds value.** Optionally, a refresh control can include a title. In most cases, this is unnecessary, as the animation of the control indicates that content is loading. If you do include a title, don’t use it to explain how to perform a refresh. Instead, provide information of value about the content being refreshed. A refresh control in Podcasts, for example, uses a title to tell people when the last podcast update occurred.

> **값이 추가될 때만 작은 제목을 제공하세요.** 선택적으로, refresh control은 제목을 포함할 수 있습니다. 대부분의 경우, control의 애니메이션이 콘텐츠가 로딩되고 있는 것을 나타내므로 불필요합니다. 제목을 포함하고자 한다면, 새로 고침 하는 방법을 설명하기 위해서 그것을 사용하지 마세요. 그 대신에, 새로 고침 된 콘텐츠의 값의 정보를 제공하세요. 예를 들어, Podcasts 앱의 refresh control은 사용자에게 언제 마지막 podcast 업데이트가 발생했는지 알려주기 위해서 제목을 사용합니다.

For developer guidance, see [UIRefreshControl](https://developer.apple.com/documentation/uikit/uirefreshcontrol).

> 개발자 가이드는 다음 문서를 참조하세요.