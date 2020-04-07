# Buttons
Buttons initiate app-specific actions, have customizable backgrounds, and can include a title or an icon. The system provides a number of predefined button styles for most use cases. You can also design fully custom buttons.

> 버튼은 앱 별로 동작을 시작하고, 사용자 지정의 배경을 가지며, 제목 또는 아이콘을 가질 수 있습니다. 시스템은 사용되는 대부분의 경우, 많은 수의 이미 지정되어 있는 버튼의 스타일을 제공합니다. 그뿐만 아니라, 완전히 커스텀 한 버튼을 디자인할 수도 있습니다.



For developer guidance, see [UIButton](https://developer.apple.com/documentation/uikit/uibutton).

> UIButton과 관련된 가이드는 다음 문서를 확인하세요.



### System Buttons

System buttons often appear in navigation bars and toolbars, but may be used anywhere.

> 시스템  버튼들은 종종 내비게이션 바 및 툴바에 보이지만, 어디든 사용될 수 있습니다.

<img width="273" alt="1" src="https://user-images.githubusercontent.com/40762111/78660526-37bc2d80-7908-11ea-89c9-d7dc7be99590.png">

**Use verbs in titles.** An action-specific title shows that a button is interactive and says what happens when you tap it.

> **제목으로 동사를 사용하세요.** 액션 별 제목은 버튼이 상호작용하며 탭 했을 때 어떤 일이 일어나는지를 보여줍니다.



**Use title-case for titles.** Capitalize every word except articles, coordinating conjunctions, and prepositions of four or fewer letters.

> **제목으로 타이틀 케이스(전치사, 관사 등을 제외한 제목의 모든 단어를 대문자로 표기하는 방법)를 사용하세요.** 기사, 꾸미는 접속사 및 4자 이하의 전치사를 제외하고 모든 단어를 대문자로 표시하세요.



**Keep titles short.** Overly long text can crowd your interface and may get truncated on smaller screens.

> **제목을 짧게 유지하세요.** 너무 긴 텍스트는 인터페이스를 혼잡하게 할 수 있고, 작은 화면에서 생각될 수 있습니다.



**Consider adding a border or a background only when necessary.** By default, a system button has no border or background. In some content areas, however, a border or background is necessary to denote interactivity. In the Phone app, bordered number keys reinforce the traditional model of making a call, and the background of the Call button provides an eye-catching target that’s easy to hit.

> **필요한 경우에만, 경계나 배경을 넣으세요.** 기본적으로, 시스템 버튼은 경계나 배경이 없습니다. 하지만 몇몇의 콘텐츠 영역의 경우, 인터랙티브를 보여주기 위해서 경계나 배경이 필요합니다. 스마트폰 앱에서, 경계가 있는 숫자 키는 전화하기의 전통적인 모델을 보강하고, 전화 앱 버튼의 배경은 터치하기 쉬워 눈을 사로잡는 타겟을 제공합니다.



For developer guidance, see the [UIButtonTypeSystem](https://developer.apple.com/documentation/uikit/uibuttontype/uibuttontypesystem) button type of [UIButton](https://developer.apple.com/documentation/uikit/uibutton).

> UIButton의 UIButtonTypeSystem 버튼 타입과 관련된 문서를 다음을 참조하세요.



### Detail Disclosure Buttons

A Detail Disclosure button opens a view—typically, a modal view—containing additional information or functionality related to a specific item onscreen. Although you can use them in any type of view, Detail Disclosure buttons are commonly used in tables to access information about specific rows.

> Detail Disclosure 버튼은 줄 모달 뷰를 여는데, 추가적인 정보 또는 화면의 구체적인 아이템과 관련된 기능을 포함합니다. 뷰의 종류에 관계없이 사용할 수 있지만, Detail Disclosure 버튼은 보통 특정 rows에서의 정보에 접근하기 위해서 tables에서 사용됩니다.

<img width="273" alt="2" src="https://user-images.githubusercontent.com/40762111/78660532-38ed5a80-7908-11ea-8af6-8249fdb1657f.png">

**Use Detail Disclosure buttons appropriately in tables.** When a Detail Disclosure button is present in a table row, tapping the button shows additional information. Tapping elsewhere selects the row or results in app-defined behavior. If you want people to tap the entire row to see additional detail, don’t use a Detail Disclosure button. Instead, use a disclosure indicator accessory control. See [disclosureIndicator](https://developer.apple.com/documentation/uikit/uitableviewcell/accessorytype/disclosureindicator) in [UITableViewCell](https://developer.apple.com/documentation/uikit/uitableviewcell).

> **Tables에서 적절하게 Detail Disclosure 버튼을 사용하세요.** Detail Disclosure 버튼이 table row에 있을 때, 버튼을 탭 하면 추가적인 정보를 보여줍니다. 다른 곳을 탭 하는 것은 row을 선택하거나, 앱에서 정의한 동작을 하게 됩니다. 사용자가 row의 전체를 탭 했을 때 추가적인 세부 사항을 보여주고 싶다면, Detail Disclosure 버튼을 사용하지 마세요. 대신, disclouse indicator accessory control을 사용하세요. UITableViewCell의 disclosureIndicator와 관련된 문서를 다음을 참조하세요.



For developer guidance, see the [UIButtonTypeDetailDisclosure](https://developer.apple.com/documentation/uikit/uibuttontype/uibuttontypedetaildisclosure) button type of [UIButton](https://developer.apple.com/documentation/uikit/uibutton).

> UIButton의 UIButtonTypeDetailDisclosure 버튼 타입과 관련된 문서를 다음을 참조하세요.



### Info Buttons

An Info button reveals configuration details about an app, sometimes on the back of the current view, after flipping the view around. Info buttons come in two styles—light and dark. Pick the style that best coordinates with your app’s design and doesn’t get lost onscreen.

> Info 버튼은 뷰를 뒤집은 후(아래 사진의 구글맵 지금은 모달 뷰인 듯), 앱과 관련된 환경 설정 세부 정보를 알려주고, 때로 현재 뷰의 뒤에 표시하기도 합니다. Info 버튼은 라이트, 다크 두 가지 스타일이 있습니다. 앱 디자인과 가장 어울리는 스타일을 선택하여 화면에서 사라지지 않게 하세요.

<img width="273" alt="3" src="https://user-images.githubusercontent.com/40762111/78660537-3985f100-7908-11ea-8c03-965bd2547e12.png">

For developer guidance, see the [UIButtonTypeInfoLight](https://developer.apple.com/documentation/uikit/uibuttontype/uibuttontypeinfolight) and [UIButtonTypeInfoDark](https://developer.apple.com/documentation/uikit/uibuttontype/uibuttontypeinfodark) button types of [UIButton](https://developer.apple.com/documentation/uikit/uibutton).

> UIButton의 UIButtonTypeInforLight 및 UIBUttonTypeInforDark 버튼 타입과 관련된 내용은 다음 문서를 참조하세요.



### Add Contact Buttons

Users can tap an Add Contact button to browse a list of existing contacts and to select one for insertion into a text field or other view. In Mail, for example, you can tap the Add Contact button in the To field of a message to select a recipient from your list of contacts.

> 사용자는 Add Contact 버튼을 탭 하여 현재 연락처 목록을 확인할 수 있고, 하나를 선택하여 text field 혹은 다른 뷰에 추가할 수 있습니다. 예를 들어, 메일 앱의 메시지의 To field에서 Add Contact 버튼을 탭 하여 연락처 목록에서 수신인을 선택할 수 있습니다.



<img width="273" alt="4" src="https://user-images.githubusercontent.com/40762111/78660540-3ab71e00-7908-11ea-812b-00f92d17723d.png">

**Allow keyboard entry in addition to the Add Contact button.** The Add Contact button provides an alternative, not a replacement, to typing contact information. It’s fine to provide it as a shortcut for adding existing contacts, but let people enter contact information with the keyboard too.

> **Add Contact 버튼 이외에 키보드 입력을 허용하세요.** Add Contact 버튼은 연락처 정보를 입력하기 위해서 대체가 아니라 대안을 제공합니다. 연락처를 추가하기 위해서 단축키로 제공하는 것도 좋지만, 사용자는 키보드로 연락처 정보를 입력하기도 합니다.



For developer guidance, see the [UIButtonTypeContactAdd](https://developer.apple.com/documentation/uikit/uibuttontype/uibuttontypecontactadd) button type of [UIButton](https://developer.apple.com/documentation/uikit/uibutton).

> UIButton의 UIButtonTypeContactAdd 관련된 내용은 다음 문서를 참조하세요.