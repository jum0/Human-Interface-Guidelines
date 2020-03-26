# Typography
Apple provides two type families you can use in your iOS apps.

> Appledms iOS 앱에서 사용할 수 있는 두 가지 폰트 묶음을 제공합니다.



**San Francisco (SF).** San Francisco is a sans serif type family that includes SF Pro, SF Pro Rounded, SF Mono, SF Compact, and SF Compact Rounded. SF Pro is the system font in iOS, macOS, and tvOS; SF Compact is the system font in watchOS. Designed to match the visual clarity of the platform UIs, the system fonts are legible and neutral.

> San Francisco는 sans serif(serif(글자 끝에 꼬리같이 있는 부분)가 없는) 폰트 묶음으로, SF Pro, SF Pro Rounded, SF Mono, SF Compact, SF Compact Rounded 를 가지고 있습니다. SF Pro는 iOS, macOS 및 tvOS의 기본 폰트입니다; SF Compact는 watchOS의 기본 폰트입니다. 플랫폼 UIs의 시각적으로 선명함에 맞추어 설계되어, 기본 폰트는 읽기 쉬우며 중립적입니다.

![The phrase 'The quick brown fox jumped over the lazy dog.' shown in San Francisco Pro.](https://developer.apple.com/design/human-interface-guidelines/ios/images/sf-pro-text-regular_2x.png)

**New York (NY).** New York is a serif typeface that provides a unique tone designed to complement the SF fonts. NY works as well in a graphic display context (at large sizes) as it does in a reading context (at text sizes).

> New York은 serif 활자체로 SF 폰트를 보완하기 위해 설계된 독특한 톤을 제공한다. NY는 읽는 환경(글자 크기)뿐만 아니라, 그래픽 디스플레이 환경(큰 사이즈)에서도 적합합니다.



![The phrase 'The quick brown fox jumped over the lazy dog.' shown in New York.](https://developer.apple.com/design/human-interface-guidelines/ios/images/new-york_2x.png)

You can download the San Francisco and New York fonts [here](https://developer.apple.com/fonts/).

> San Francisco와 New York 폰트는 이곳에서 다운받을 수 있습니다.



Because SF Pro and NY are compatible, there are many ways you can incorporate typographic contrast and diversity into your iOS interfaces while maintaining a consistent look and feel. For example, using both typefaces can help you create stronger visual hierarchies or highlight semantic differences in content.

> SF Pro와 NY는 호환되기 때문에, 일관된 모양이나 느낌을 유지하면서 iOS 인터페이스 타이포그래픽 대비와 다양성을 통합할 수 있는 여러 방법이 있습니다. 예를 들어, 두 활자체는 강한 시각적인 계층 구조를 만들거나 콘텐츠의 의미적 차이를 강조하는데 도움을 줄 수 있습니다.



Apple-designed typefaces support an extensive range of weights, sizes, styles, and languages, so you can design comfortable and beautiful reading experiences throughout your app. When you use text styles with the system fonts, you also get support for Dynamic Type and the larger accessibility type sizes, which let people choose the text size that works for them. For specific values, see [Dynamic Type Sizes](https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/typography/#dynamic-type-sizes) and [Larger Accessibility Type Sizes](https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/typography/#larger-accessibility-type-sizes). Size information, including tracking values, is also available in the Sketch, Photoshop, and Adobe XD [Apple Design Resources](https://developer.apple.com/design/resources/#ios-apps) for iOS.

> Apple이 설계한 서체는 넓은 범위는 굵기, 크기, 스타일 및 언어 등을 지원하여, 앱에서 편하고 아름다운 읽기 경험을 디자인할 수 있습니다. 글자 스타일을 기본 폰트로 사용하면, Dynamic Type과 사용자가 적합한 텍스트의 크기를 선택하는 더 큰 접근성 type size 또한 지원합니다. 구체적인 수치는 다음 문서를 확인하세요. 추적 값을 포함하여 크기 정보는 iOS용 Sketch, Photoshop 및 Adobe XD 애플 디자인 리소스에서도 확인할 수 있습니다.



The system defines APIs that make it easy to use the SF and NY typefaces; for developer guidance, see the [withDesign method](https://developer.apple.com/documentation/uikit/uifontdescriptor/3151797-withdesign) and [SystemDesign structure](https://developer.apple.com/documentation/uikit/uifontdescriptor/systemdesign) of [UIFontDescriptor](https://developer.apple.com/documentation/uikit/uifontdescriptor).

> 시스템은 API로 SF와 NY 서체를 쉽게 사용하도록 정의합니다. 개발자 가이드는 다음 문서를 확인하세요.



### SF Pro and SF Compact

The flexibility of the system fonts helps you achieve optimal legibility at every point size and gives you the breadth and depth you need for precision typesetting throughout your app.

> 시스템 폰트의 유연성은 모든 포인트의 크기의 최적의 가독성을 위해 도움을 주고, 앱 전체적으로 정밀하게 타이핑하는데 필요한 너비와 깊이를 제공합니다.



SF Pro and SF Compact support:

- Over one hundred languages using Latin, Greek, and Cyrillic scripts

  > 라틴어, 그리스어, 키릴 문자의 스크립트를 사용하는 100개 이상의 언어 지원

- Nine weights — from Ultralight to Black — in both uprights and italics

  > 수직인 글씨와 이태릭체 모두 Ultralight부터 Black까지 아홉 가지의 폰트 굵기 지원

- Two optical sizes — Text and Display

  > 텍스트와 디스플레이에 최적화된 사이즈 지원

- Variable letter spacing that automatically adjusts based on the size of the text

  > 텍스트의 크기에 따라 자동으로 조정되는 가변 문자 간격 지원

- Small capitals, fractions, and inferior and superior numerals

  > Small capitals(대문자로 지정된 서체의 대문자보다 길이가 짧은 대문자), 분수, 위쪽과 아래쪽 숫자(x^4에서 4 또는, H2O에서 2) 지원

For developer guidance, see the [default property](https://developer.apple.com/documentation/uikit/uifontdescriptor/systemdesign/3151799-default) of the [SystemDesign structure](https://developer.apple.com/documentation/uikit/uifontdescriptor/systemdesign).

> 개발자 가이드는 다음 문서를 참조하세요. 



### SF Pro Rounded and SF Compact Rounded

The rounded variant of the system fonts can help you coordinate your text style with the appearance of soft or rounded UI elements, or to provide an alternative typographic voice.

> 시스템 폰트의 원형의 형태의 변화는 텍스트 스타일에 부드러운 모양 또는 둥근 UI요소, 또는 대안적인 타이포그래픽 보이스를 제공하여 조정할 수 있다.



SF Pro Rounded and SF Compact Rounded support:

- Over one hundred languages using Latin, Greek, and Cyrillic scripts

  > 라틴어, 그리스어, 키릴 문자의 스크립트를 사용한 100개 이상의 언어 지원

- Uprights in nine weights — from Ultralight to Black

  > 수직인 글씨 Ultralight부터 Black까지 아홉 가지의 폰트 굵기 지원

- Variable letter spacing that automatically adjusts based on the size of the text

  > 텍스트의 크기에 따라 자동으로 조정되는 가변 문자 간격 지원

- Small capitals, fractions, and inferior and superior numerals

  > Small capitals(대문자로 지정된 서체의 대문자보다 길이가 짧은 대문자), 분수, 위쪽과 아래쪽 숫자(x^4에서 4 또는, H2O에서 2) 지원

For developer guidance, see the [rounded property](https://developer.apple.com/documentation/uikit/uifontdescriptor/systemdesign/3151800-rounded) of the [SystemDesign structure](https://developer.apple.com/documentation/uikit/uifontdescriptor/systemdesign).

> 개발자 가이드는 다음 문서를 참조하세요.



### SF Mono

SF Mono is a monospaced variant of San Francisco — that is, a typeface in which all characters are equal in width. You typically use a monospaced typeface when you want to align columns of text, such as in a coding environment. For example, Xcode and Swift Playgrounds use SF Mono by default.

> SF Mono는 San Francisco의 고정된 너비의 변형으로, 모든 문자의 폭이 동일한 서체입니다. 대표적으로 코딩 환경과 같이 텍스트의 column을 정렬하고자 할 때, monospaced 서체를 이용합니다. 예를 들어, Xcode와 Swift Playgroudns는 기본적으로 SF Mono를 사용합니다.



**NOTE**

SF Pro uses the OpenType tabular lining feature to support the display of monospaced numbers and currencies.

> SF Pro는 고정된 너비의 숫자와 통화의



SF Mono supports:

- Over one hundred languages using Latin, Greek, and Cyrillic scripts

  > dfdf

- Six weights — from Light to Heavy — in both uprights and italics

  > Dfdfd

- Monospacing across all weights (that is, changing the font weight doesn't cause the text to reflow)

  > Dffd

For developer guidance, see the [monospaced property](https://developer.apple.com/documentation/uikit/uifontdescriptor/systemdesign/3152921-monospaced) of the [SystemDesign structure](https://developer.apple.com/documentation/uikit/uifontdescriptor/systemdesign).

> Dfdf



### New York

New York is a classical serif typeface you can use in the interface or to provide a traditional reading experience.

> Dfdf



NY supports:

- Over one hundred languages using Latin, Greek, and Cyrillic scripts

  > Dfdf

- Six weights — from Regular to Black — in both uprights and italics

  > Dfdf

- Four optical sizes — Small, Medium, Large, and Extra Large

  > dfdf

- Variable letter spacing that automatically adjusts based on the size of the text

  > Did

For developer guidance, see the [serif property](https://developer.apple.com/documentation/uikit/uifontdescriptor/systemdesign/3152922-serif) of the [SystemDesign structure](https://developer.apple.com/documentation/uikit/uifontdescriptor/systemdesign).

> Off



### Choosing Fonts to Enhance Your App

**Use built-in text styles whenever possible.** The built-in text styles let you express content in ways that are visually distinct, while retaining optimal legibility. These styles—including headline, body, callout, and several sizes of title—are based on the system fonts and let you take advantage of key typographic features, such as Dynamic Type, which automatically adjusts tracking and leading for every font size. For developer guidance, see [UIFontTextStyle](https://developer.apple.com/documentation/uikit/uifonttextstyle).

> dfdf



**Emphasize important information.** Use font weight, size, and color to highlight the most important information in your app.

> dfdf



**Prioritize content when responding to text-size changes.** Not all content is equally important. When someone chooses a larger size, they want to make the content they care about easier to read; they don’t always want every word on the screen to be larger.

> dfdfd



**Use the correct font variant in interface mockups.** When you use San Francisco for text in standard controls like buttons and labels, iOS automatically applies the most appropriate variant based on the point size and the current accessibility settings. In interface mockups, use the following text sizes to choose the correct size and adjust the spacing between letters as needed.

> dfdf

- For SF, use Text for text that's smaller than 20 points; use Display for text that's 20 points or larger.

  > dfdf

- For NY, use Small for text that's smaller than 20 points, Medium for text between 20 and 35 points, large for text between 36 and 53 points, and Extra Large for text that's 54 points or larger.

  > dfdfd

**NOTE**

iOS uses San Francisco as the system font for Latin, Greek and Cyrillic alphabets, and a variety of other typefaces for other scripts.

> dfd



**Minimize the number of typefaces you use in your interface.** Mixing too many different typefaces can make your app seem fragmented and sloppy.

> dfdf



**Make sure custom fonts are legible.** Custom typefaces are supported on iOS, but may be tough to read, especially if they have stylistic attributes that make letterforms hard to discern when displayed at small sizes. Unless your app has a compelling need for a custom font — such as for branding purposes or to create an immersive gaming experience — it’s usually best to stick with the system fonts. Consider using a custom font for display text only; if you do use it for reading or interface text, make sure it’s legible, even at small sizes.

> dfdf



**Implement accessibility features for custom fonts.** System fonts automatically react to accessibility features like bold text and larger type. Implement the same behavior in apps that use custom fonts by making sure accessibility features are enabled and registering for notifications when they change. See [Text Size and Weight](https://developer.apple.com/design/human-interface-guidelines/accessibility/overview/text-size-and-weight/).

> dfdf



### Dynamic Type Sizes

Dynamic Type provides additional flexibility by letting readers choose their preferred text size. Here are the weight, size, and leading values for each text style at different Dynamic Type sizes.

> Dfdf

#### 

S - Size(Points) / L - Leading(Points)

|             |            | xSmall |       | Small |       | Medium |       | Large<br />(Default) |       | xLarge |       | xxLarge |       | xxxLarge |       |
| :---------: | :--------: | :----: | :---: | :---: | :---: | :----: | :---: | :------------------: | :---: | :----: | :---: | :-----: | :---: | :------: | :---: |
|  **Style**  | **Weight** | **S**  | **L** | **S** | **L** | **S**  | **L** |        **S**         | **L** | **S**  | **L** |  **S**  | **L** |  **S**   | **L** |
| Large Title |  Regular   |   31   |  38   |  32   |  39   |   33   |  40   |          34          |  41   |   36   |  43   |   38    |  46   |    40    |  48   |
|   Title 1   |  Regular   |   25   |  31   |  26   |  32   |   27   |  33   |          28          |  34   |   30   |  37   |   32    |  39   |    34    |  41   |
|   Title 2   |  Regular   |   19   |  24   |  20   |  25   |   21   |  26   |          22          |  28   |   24   |  30   |   26    |  32   |    28    |  34   |
|   Title 3   |  Regular   |   17   |  22   |  18   |  23   |   19   |  24   |          20          |  25   |   22   |  28   |   24    |  30   |    26    |  32   |
|  Headline   | Semi-Bold  |   14   |  19   |  15   |  20   |   16   |  21   |          17          |  22   |   19   |  24   |   21    |  26   |    23    |  29   |
|    Body     |  Regular   |   14   |  19   |  15   |  20   |   16   |  21   |          17          |  22   |   19   |  24   |   21    |  26   |    23    |  29   |
|   Callout   |  Regular   |   13   |  18   |  14   |  19   |   15   |  20   |          16          |  21   |   18   |  23   |   20    |  25   |    22    |  28   |
|   Subhead   |  Regular   |   12   |  16   |  13   |  18   |   14   |  19   |          15          |  20   |   17   |  22   |   19    |  24   |    21    |  28   |
|  Footnote   |  Regular   |   12   |  16   |  12   |  16   |   12   |  16   |          13          |  18   |   15   |  20   |   17    |  22   |    19    |  24   |
|  Caption 1  |  Regular   |   11   |  13   |  11   |  13   |   11   |  13   |          12          |  16   |   14   |  19   |   16    |  21   |    18    |  23   |
|  Caption 2  |  Regular   |   11   |  13   |  11   |  13   |   11   |  13   |          11          |  13   |   13   |  18   |   15    |  20   |    17    |  22   |

Point size based on image resolution of 144ppi for @2x and 216ppi for @3x designs.







### Larger Accessibility Type Sizes

In addition to the standard dynamic type sizes, the system offers a number of even larger sizes for users with accessibility needs. Here are the weight, size, and leading values for each text style at the larger accessibility type sizes.

> Did



S - Size(Points) / L - Leading(Points)

|             |            |  AX1  |       |  AX2  |       |  AX3  |       |  AX4  |       |  AX5  |       |
| :---------: | :--------: | :---: | :---- | :---: | :---: | :---: | ----- | :---: | :---: | :---: | :---: |
|  **Style**  | **Weight** | **S** | **L** | **S** | **L** | **S** | **L** | **S** | **L** | **S** | **L** |
| Large Title |  Regular   |  44   | 52    |  48   |  57   |  52   | 61    |  56   |  66   |  60   |  70   |
|   Title 1   |  Regular   |  38   | 46    |  43   |  51   |  48   | 57    |  53   |  62   |  58   |  68   |
|   Title 2   |  Regular   |  34   | 41    |  39   |  47   |  44   | 52    |  50   |  59   |  56   |  66   |
|   Title 3   |  Regular   |  31   | 38    |  37   |  44   |  43   | 51    |  49   |  58   |  55   |  65   |
|  Headline   | Semi-Bold  |  28   | 34    |  33   |  40   |  40   | 48    |  47   |  56   |  53   |  62   |
|    Body     |  Regular   |  28   | 34    |  33   |  40   |  40   | 48    |  47   |  56   |  53   |  62   |
|   Callout   |  Regular   |  26   | 32    |  32   |  39   |  38   | 46    |  44   |  52   |  51   |  60   |
|   Subhead   |  Regular   |  25   | 31    |  30   |  37   |  36   | 43    |  42   |  50   |  49   |  58   |
|  Footnote   |  Regular   |  23   | 29    |  27   |  33   |  33   | 40    |  38   |  46   |  44   |  52   |
|  Caption 1  |  Regular   |  22   | 28    |  26   |  32   |  32   | 39    |  37   |  44   |  43   |  51   |
|  Caption 2  |  Regular   |  20   | 25    |  24   |  30   |  29   | 35    |  34   |  41   |  40   |  48   |

Point size based on image resolution of 144ppi for @2x and 216ppi for @3x designs.