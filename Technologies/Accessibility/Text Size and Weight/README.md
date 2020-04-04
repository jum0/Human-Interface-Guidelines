# Text Size and Weight
When designing an inclusive app, keep text size, weight, and layout in mind for clarity and readability. To learn how color and contrast can affect the legibility of text in your app, see [Color and Contrast]([https://github.com/jum0/Human-Interface-Guidelines/tree/master/Accessibility/Color%20and%20Contrast).

> 다양한 앱을 디자인할 때, 명료함과 가독성을 위해서 테스트 크기와 두께 및 레이아웃을 기억하세요. 색과 대비가 앱에서 텍스트의 가독성에 어떻게 영향을 미칠 수 있는지 배우려면, 다음 문서를 확인하세요.



**Use Dynamic Type and test that your app's layout adapts to all accessibility font sizes.** Dynamic Type lets people pick the font size that works for them. Verify that your design can scale and is legible at all accessibility font sizes for both text and glyphs. You can download the dynamic type size tables in the Sketch, Photoshop, and Adobe XD [Apple Design Resources](https://developer.apple.com/design/resources/).

> **Dynamic Type을 사용하고 앱의 레이아웃이s 모든 접근성의 폰트 크기에 적용되는지 확인해 보세요.** Dynamic Type은 사용자가 사용하기에 적합한 폰트 크기를 고를 수 있도록 도와줍니다. 디자인의 크기를 조정할 수 있고, 디자인이 텍스트와 문자에서 모든 접근성 폰트 크기로 읽을 수 있는지 확인하세요. Sketch, Photoshop, Adobe XD에서 dynamic type size 표를 다운 받을 수 있습니다.

<img width="552" alt="스크린샷 2020-03-28 오후 11 29 01" src="https://user-images.githubusercontent.com/40762111/77825359-190da800-714c-11ea-84a4-55c9d8d4f387.png">

**As font size increases, avoid truncating text.** It's best when people can simply scroll to see the same amount of text that's visible at the default font size. Don't truncate text unless people can open a separate view to read the rest of the content.

> **폰트의 크기가 커짐에 따라 텍스트 truncating(줄여서 ... 되는 것) 하는 것을 피하세요.** 사용자가 간단하게 scrol l하여 기본 폰트 크기로 보이는 텍스트의 같은 양을 볼 수 있는 것이 가장 좋습니다. 사용자가 나머지의 콘텐츠를 읽기 위해서 별도의 뷰를 열 수 없다면, 텍스트를 자르지 마세요.



**Increase the size of meaningful glyphs as font size increases.** If you use glyphs to communicate important information, make sure the glyphs are easy to view at larger font sizes, too.

> **폰트의 크기가 커짐에 따라 의미 있는 문자의 크기도 키우세요.** 중요한 정보를 전달하기 위해서 문자를 사용한다면, 문자는 폰트 크기가 큰 경우에도 쉽게 볼 수 있어야 합니다.

<img width="552" alt="스크린샷 2020-03-28 오후 11 29 11" src="https://user-images.githubusercontent.com/40762111/77825360-19a63e80-714c-11ea-8559-486c48cec577.png">

**Maintain a consistent information hierarchy regardless of the user’s font size choice.** For example, keep primary elements towards the top of the screen even when the font size is very large, so that people don’t lose track of these elements.

> **사용자의 폰트 크기 선택에 관계없이 일관된 정보 구졸 유지하세요.** 예를 들어, 폰트의 크기가 매우 큰 경우에도 화면의 가장 위에 주요 요소를 유지하여, 사용자가 이러한 요소들을 계속 볼 수 있도록 하세요.



**Use regular or heavy font weights in your app.** Use Regular, Medium, Semi-Bold, or Bold font weights, because they are easier to see. Avoid UltraLight, Thin, and Light font weights, which can be more difficult to see.

> **앱에서 regular 혹은 heavy 폰트의 두께를 사용하세요.** Regular, Medium, Semi-Bold 또는 Bold 폰트 두께는 보기 쉽습니다. UltraLight, Thin 및 Light 폰트 두께는 보기 어렵습니다.



**Ensure that your app responds correctly and looks good when users enable bold text.** People turn on the bold text accessibility setting to make text and glyphs easier to see. In response, your app should make all text bolder and give all glyphs an increased stroke weight.

> **사용자가 bold 텍스트를 사용할 때, 올바르게 응답하고 좋아 보이도록 유지하세요.** 사용자는 텍스트와 문자를 보기 쉽게 하기 위해서 bold 텍스트 접근성 설정을 기능을 켭니다. 이에 응답해서, 앱에서 모든 텍스트를 bolder 하게 하고, 모든 문자를 두껍게 해야 합니다.

<img width="552" alt="스크린샷 2020-03-28 오후 11 29 20" src="https://user-images.githubusercontent.com/40762111/77825361-1ad76b80-714c-11ea-9553-1b5a4ef422e7.png">

**Make sure custom fonts are legible.** Custom typefaces can sometimes be difficult to read. Unless your app has a compelling need for a custom font, such as for branding purposes or to create an immersive gaming experience, it’s usually best to use the system fonts. If you do use a custom font, make sure it’s easy to read, even at small sizes.

> **커스텀 폰트를 읽기 쉽게 해야 합니다.** 커스텀 글꼴은 때때로 읽기 어려울 수 있습니다. 브랜딩의 목적 혹은 게임과 같이 몰입적인 경험을 만들기 위해서 커스텀 폰트를 사용하는 것이 강제되는 것이 아니라면, 보통은 시스템 폰트를 사용하는 것이 가장 좋습니다. 커스텀 폰트를 사용하면, 작은 사이즈에서도 읽기 쉽도록 유지하세요.



**Avoid full text justification.** The whitespace created by fully justified text can create patterns that make it difficult for many people to read and focus on the text. Left justification (or right justification in right-to-left languages) provides a framing reference for people with learning and literacy challenges, such as dyslexia.

> **전체 텍스트 맞춤을 피하세요.** 전체적으로 나란히 맞춰지는 텍스트로 생겨난 여백은 사용자가 텍스트를 읽고 집중하는 데 어려움을 느끼게 할 수 있습니다. 좌측 정렬(오른쪽에서 시작하는 언어의 우측 정렬)은 난독증과 같이 학습능력과 읽고 쓰는 능력에 어려움을 겪는 사용자에게 framing reference를 제공합니다.



**Avoid using italics or all caps for long passages of text.** Italics and all caps are great for occasional emphasis, but overuse of these styles makes text hard to read.

> **긴 글에 이태릭체나 대문자를 모두 사용하는 것은 피하세요.** 이태릭체와 모든 대문자 사용은 때때로 강조하는 것에 좋은 선택이지만, 이러한 스타일의 과한 사용은 텍스트를 읽기 어렵게 만들 수 있습니다.