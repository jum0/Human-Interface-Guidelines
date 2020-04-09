# User Interaction
Assistive technologies like VoiceOver and accessibility features like display accommodations expand the ways people can interact with their devices. Because these technologies and features integrate with system-provided interactions, it's essential that you support the system interactions correctly in your app.

> VoiceOver와 같은 보조 기술 및 [display accomodations](https://ios.gadgethacks.com/how-to/cant-find-accessibility-menu-its-options-ios-13-got-huge-update-worth-checking-out-0198392/)와 같은 접근성 특징은 사용자들이 기기와 인터랙션 할 수 있는 방식을 확장합니다. 이러한 기술과 특징이 시스템에서 제공하는 인터랙션과 결합하기 때문에, 앱에서 적절하게 시스템 인터랙션을 지원하는 것을 필수적입니다.



### Gestures

**Give all controls and interactive elements a hit target that measures at least 44pt x 44pt.** People with limited mobility need larger hit targets to help them interact with your app. Controls that are too small can be frustratingly difficult for all users to hit.

> **모든 controls와 인터랙티브한 요소들이 최소한 44pt * 44pt의 크기의 타깃이 되도록 하세요. ** 기동성에 제한이 있는 사용자들은 더 큰 타깃으로 앱과 인터랙션 하는 것을 필요로 합니다. 너무 작은 controls는 모든 사용자들이 접근하기 불만스러울 정도로 어려울 수 있습니다.



**Don’t override the platform gestures.** People expect system gestures—such as swiping down to reveal Notification Center or the macOS trackpad gestures available in System Preferences—to work regardless of the app they’re using.

> **플랫폼 제스처와 중복되지 않도록 하세요.** 사용자들은 Notification Center을 보기 위해서 아래쪽으로 스와이프 하거나, 사용자들이 사용하는 애플리케이션과 관계없이 작업하기 위해 시스템 환경 설정에서 사용 가능한 macOS 트랙 패드 제스처 등의 시스템 제스처를 기대합니다. 



**Prefer simplified gestures for interaction.** Complex gestures such as multifinger gestures, long presses, or repeated button presses can be challenging for many people. Using the simplest gestures possible improves the experience for everyone who interacts with your app.

> **인터랙션을 위한 간단한 제스처를 선호하세요.** 여러 손가락을 사용하는 제스처, 길게 누르기 또는 반복된 버튼 누르기 등과 같은 복잡한 제스처는 많은 사람들에게 어려울 수 있습니다. 가능한 매우 간단한 제스처를 사용하는 것을 앱과 인터랙션 하는 모든 사람들의 경험을 향상시켜 줍니다.



**Provide alternative ways to perform gesture-based actions.** Include an option for people who may not be able to perform a specific gesture. For example, if swiping deletes a row in a table, you should also give people an alternative way to delete items through an edit mode or by offering a Delete button in an item detail view.

> **제스처 기반의 동작을 수행하기 위해서 대안을 제공하세요.** 특정 제스처를 수행할 수 없는 사용자들을 위한 선택권을 포함하세요. 예를 들어, table에서 스와이프 하여 row를 삭제하면, 사용자에게 편집 모드를 통해 아이템을 삭제하거나 아이템 상세 화면에서 삭제 버튼을 제공하는 방식의 대안을 제공해야 합니다. 



<img width="273" alt="스크린샷 2020-04-09 오후 1 36 14" src="https://user-images.githubusercontent.com/40762111/78858381-3d7c5500-7a67-11ea-8773-7aecd068bd3e.png">

**Make drag and drop accessible in your iOS app.** When you use the accessibility APIs to identify drag sources and drop targets in your app, assistive technologies can help people drag and drop onscreen items. For developer guidance, see [accessibilityDragSourceDescriptors](https://developer.apple.com/documentation/objectivec/nsobject/2891001-accessibilitydragsourcedescripto) and [accessibilityDropPointDescriptors](https://developer.apple.com/documentation/objectivec/nsobject/2891048-accessibilitydroppointdescriptor).

> **iOS 앱에서 drag와 drop 접근성을 만드세요.** 앱에서 drag sources와 drop targets을 구분하기 위해서 접근성 APIs을 사용할 때, 보조 기술은 사용자가 화면 속 아이템을 drag 및 drop 할 수 있도록 돕습니다. accesibilityDrageSourceDescriptors  accessibilityDropPointDescriptors와 관련된 가이드는 다음 문서를 확인하세요.



**Don't require 3D Touch (iOS) or Force Touch (Apple Watch) to access your app's core functionality.** Not everyone can press the screen to get the additional functionality provided by 3D Touch and Force Touch. Ensure that all users can perform important actions in your app even if they can't use 3D Touch or Force Touch.

> **앱의 중요한 기능에 접근하기 위해서 3D Touch (iOS) 또는 Force Touch (Apple Watch)를 요구하지 마세요.** 3D Touch와 Force Touch로 제공되는 추가적인 기능에 접근하기 위해서 모든 사용자들이 화면을 누를 수 있는 것은 아닙니다. 모든 사용자들이 3D Touch 혹은 Force Touch를 사용할 수 없어도, 앱에서 중요한 동작을 수행할 수 있도록 유지하세요.



To learn more about gestures, see [Clicks and Gestures (macOS)](https://developer.apple.com/design/human-interface-guidelines/macos/user-interaction/mouse-and-trackpad/#clicks-and-gestures/), [Gestures (tvOS)](https://developer.apple.com/design/human-interface-guidelines/tvos/remote-and-controllers/remote/#gestures), [Gestures (watchOS)](https://developer.apple.com/design/human-interface-guidelines/watchos/user-interaction/gestures/), and [Gestures (iOS)](https://developer.apple.com/design/human-interface-guidelines/ios/user-interaction/gestures/).

> 제스처와 관련된 더 많은 것들은 Clicks and Gestures (macOS), Gestrues (tvOS), Gestures (watchOS) 및 Gestures (iOS) 문서를 참조하세요.



### Haptics

**Support the system-defined haptics.** Many people rely on haptics to help them interact with apps when they can't see the screen. For example, system apps play haptics to notify people when a task has succeeded or failed or when an event is about to happen. Be sure to use the system-defined haptics consistently in your app so that you don't confuse people.

> **시스템에서 정의된 haptics을 지원하세요.** 많은 사용자들은 화면을 볼 수 없을 때, 앱과 상호 작용하는 것을 돕기 위해서 haptics에 의존합니다. 예를 들어, 시스템 앱은 작업이 성공 혹은 실패했을 때나 일정이 생기자마자 사용자에게 알려주기 위해서 haptics을 동작합니다. 앱에서 시스템 정의된 haptics을 일관되게 제공하여 사용자가 혼란스럽지 않도록 유의하세요.



To learn more about system-defined haptics, see [Haptic Feedback (macOS)](https://developer.apple.com/design/human-interface-guidelines/macos/user-interaction/mouse-and-trackpad/#haptic-feedback), [Haptics (iOS)](https://developer.apple.com/design/human-interface-guidelines/ios/user-interaction/haptics/), and [Haptic Feedback (watchOS)](https://developer.apple.com/design/human-interface-guidelines/watchos/user-interaction/haptic-feedback/).

> 시스템에서 정의된 haptics과 관련된 더 많은 정보들은 Haptic Feedback (macOS), Haptics (iOS), 및 Haptic Feedback (watchOS) 문서들을 참조하세요.



### Buttons and Controls

**Characterize the accessibility of custom elements.** You can use accessibility traits (UIKit) and properties (AppKit) to tell assistive technologies how an element behaves. For example, using [button](https://developer.apple.com/documentation/uikit/uiaccessibility/uiaccessibilitytraits/1620194-button) or [NSAccessibilityButton](https://developer.apple.com/documentation/appkit/nsaccessibilitybutton) to characterize a view as a button means that VoiceOver speaks the view's description followed by the word *button*, which tells people that the view behaves like a button.

> **커스텀 요소들의 접근성을 특징으로 하세요.** 접근성 특징 (UIKit) 및 속성 (AppKit)을 사용하여 어떻게 요소가 동작하는지 보조 기술에게 알려줄 수 있습니다. 예를 들어, 버튼 혹은 NSAccessibilityButton을 사용하여 뷰를 버튼으로 나타내면, VociceOver이 button 이후에 버튼과 같은 동작하는 뷰의 설명을 사용자에게 알려줍니다.



**Use a consistent style hierarchy to communicate the relative importance of buttons.** People can turn on Button Shapes to make it easier to distinguish active buttons from surrounding content. When you use a consistent hierarchy of button styles, people can grasp the importance of buttons based on their appearance. For example, the most important buttons use a rounded rectangle shape and a color fill; secondary buttons aren't color-filled, but may display text or a glyph in the key color; and the least critical buttons use underlined text.

> **중요도가 다른 버튼들과 소통하기 위해서 일관된 스타일의 계층을 사용하세요.** 사용자들은 콘텐츠 주위의 active 한 버튼들을 더 쉽게 구별하기 위해서 Button Shapes를 켤 수 있습니다. 버튼 스타일의 일관된 계층을 사용하면,  사용자들은 버튼의 모습을 보고 그 중요성을 알 수 있습니다. 예를 들어, 가장 중요한 버튼들은 둥근 직사각형 모양이며 색으로 채워져 있습니다. 두 번째의 중요도를 지닌 버튼들은 색으로 채워져 있지 않지만, 핵심 색의 텍스트 혹은 문자를 보여줄 수 있습니다; 그리고 중요한 버튼은 최소한 밑줄이 있는 텍스트를 사용합니다.



**Prefer the system-provided switch.** UIKit provides a switch that indicates its state by the position of its knob and its fill color. For some people, however, the addition of labels makes it easier to perceive whether a switch is on or off. When you use system-provided switches, iOS automatically displays on/off glyphs within them when people turn on On/Off Labels.

> **시스템에서 제공하는 switch를 사용하는 것을 선호합니다.** UIKit은 스위치를 제공하는데 손잡이와 색이 채워진 위치로 상태를 나타냅니다. 하지만, 몇몇 사용자들에게 추가적인 글자로 스위치의 on/off 유무를 쉽게 인지할 수 있도록 도울 수 있습니다. 시스템에서 제공하는 스위치를 사용할 때, 사용자들이 On/Off 라벨을 켜면 iOS가 자동으로 그 안에 있는 문자를 보여줍니다.

<img width="564" alt="스크린샷 2020-04-09 오후 1 36 41" src="https://user-images.githubusercontent.com/40762111/78858385-3ead8200-7a67-11ea-8fc2-80ee184c4619.png">

**Consider giving links a visual indicator, such as an underline.** It’s fine to use color to indicate a link, but if you use it as the only indicator, people with color blindness may not be able to perceive the distinction. For more information about using color to communicate in your app, see [Color and Contrast](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Technologies/Accessibility/Color%20and%20Contrast).

> **밑줄과 같이 링크에 시각적인 indicator를 표시를 고려하세요.** 링크를 표시하기 위해서 색을 사용하는 것도 좋지만, indicator를 색으로만 한다면, 색맹인 사용자들은 인지하지 못할 수도 있습니다. 앱과 의사소통하기 위해서 색을 사용하는 것과 관련된 문서는 Color and Contrast를 참조하세요.



### User Input

**Let people input information by speaking instead of typing.** Adding a dictation button in a text entry field lets people choose speech as their preferred input method. If you create a custom keyboard, be sure to include a microphone key for dictation.

> **사용자가 타이핑을 하는 대신 말을 함으로써 정보를 입력할 수 있도록 하세요.** 텍스트 입력 창에 받아쓰기 버튼을 추가하는 것은 사용자가 선호하는 입력 방식으로 말하기를 선택할 수 있도록 합니다. 커스텀 키보드를 만든다면, 받아쓰기를 위해서 마이크 키를 포함하도록 하세요.



**Support Siri or Siri Shortcuts for performing important tasks by voice alone.** To learn more about enabling Siri interactions in your app, see [SiriKit](https://developer.apple.com/design/human-interface-guidelines/sirikit/).

> **중요한 작업을 목소리로만 수행하기 위해서 시리 또는 시리 단축키를 지원하세요.** 앱에서 시리 인터랙션과 관련해 더 많은 것은 SiriKit 문서를 확인하세요.



**Don’t prevent users from selecting plain text.** Many users rely on using selected text as input for text to speech (TTS) or for looking up translations.

> **사용자의 기본 텍스트 선택을 막지마세요.** 많은 사용자들이 선택한 텍스트를 text to speech (TTS) 또는 번역 검색을 위한 입력으로 사용합니다.