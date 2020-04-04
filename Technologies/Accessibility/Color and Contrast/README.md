# Color and Contrast
**Don’t rely solely on color to differentiate between objects or communicate important information.** If your app uses color to convey information, be sure to provide text labels or glyph shapes so color blind users can understand it as well.

>  **색에만 의존하여 객체를 구별하거나 중요한 정보를 전달하지 마세요.** 정보를 전달하기 위해 색을 사용한다면, 텍스트 또는 상형문자 모양을 제공하여, 색맹의 사용자가 이해할 수 있도록 하세요.



**Prefer system colors for text.** When you color text using the colors defined by [UIColor](https://developer.apple.com/documentation/uikit/uicolor) or [NSColor](https://developer.apple.com/documentation/appkit/nscolor), the text responds correctly to accessibility settings such as Invert Colors and Increase Contrast.

> **텍스트는 시스템 색상을 선호하세요.** UIColor 또는 NSColor에서 정의한 색상을 사용하여 텍스트의 색을 변경하면, 텍스트는  색 반전과 대비 증가와 같은 접근성 설정에 올바르게 응답합니다.



**Be aware of color blindness.** Many colorblind people find it difficult to distinguish blue from orange, for example, or red from green (and either red or green from gray). Avoid using these color combinations as the only way to distinguish between two states or values. For example, instead of using red and green circles to indicate offline and online, you could use a red square and a green circle. Some image-editing software includes tools that can help you proof for colorblindness.

> **색맹을 인지하세요.** 많은 색맹 사용자들은, 주황색에서 파란색을 또는 초록색에서 빨간색을(그리고 회색에서 빨간색 또는 초록색을) 구별하는 데 어려움을 느낍니다. 두 상태 또는 값을 구별하는 유일한 방법으로 이런 색상 조합을 사용하지 마세요. 예를 들어, 온라인과 오프라인 상태를 나타내기 위해 빨간색과 초록색 원을 사용하는 대신, 빨간 네모와 초록 원을 사용할 수 있습니다. 몇몇의 이미지 편집 소프트웨어는 색맹을 증명하는 도구를 가지고 있습니다.



<img width="545" alt="스크린샷 2020-03-24 오후 12 17 35" src="https://user-images.githubusercontent.com/40762111/77384758-8bd3f780-6dc9-11ea-8417-54565ce5853e.png">



**Respond correctly to Invert Colors.** People can turn on Invert Colors when they prefer to view items on a dark background. In the Smart Invert mode of Invert Colors, images, video, and full-color icons (such as app icons and nontemplate images) don't invert, and dark UI stays dark.

> **색 반전에 올바르게 응답하세요.** 사용자들은 어두운 배경에서 정보 보는 것을 선호할 때, 색 반전을 켤 수 있습니다. 색 반전의 Smart Invert 모드에서, 이미지, 비디오, 그리고 전체가 색으로 되어있는 아이콘(앱 아이콘이나 nontemplate 이미지)은 반전되지 않으며, 어두운 상태의 UI를 유지합니다.



**Use strongly contrasting colors to improve readability.** Many factors affect the perception of color, including font size and weight, color brightness, screen resolution, and lighting conditions. When you increase color contrast of visual elements like text, glyphs, and controls, you can help more people use your app in more situations. To find out if the contrast of adjacent colors in your UI meets minimum acceptable levels, use an online color calculator based on the Web Content Accessibility Guidelines (WCAG) color contrast formula.

> **가독성을 높이기 위해서 강하게 대비되는 색을 사용하세요.** 폰트의 사이즈와 굵기, 색의 밝기, 화면의 해상도 및 빛의 조건 등을 포함한 많은 요인들이 색의 인식에 영향을 미칩니다. 텍스트, 상형 문자 및 controls와 같은 시각적인 요소의 색 대비를 증가시킬 때, 더 많은 사용자들이 다양한 환경에서 사용할 수 있도록 도울 수 있습니다. UI에서 인접한 색의 대비가 최소한의 허용할만한 기준을 충족하는지 확인하기 위해서, WCAG 색 대비 공식을 이용해서 온라인 색 계산기를 활용하세요. 



**Use text size to help determine contrast.** In general, smaller or lighter-weight text needs to have greater contrast to be legible. Use the following values for guidance.

> **색의 대비 결정하는 것을 돕기 위해서 텍스트의 크기를 사용하세요.** 일반적으로, 더 작고 얇은 굵기의 텍스트는 알아보기 위해서 더 강한 대비가 요구됩니다. 다음 가이드의 값들을 활용하세요.



| Text size        | Text weight | Minimum contrast ratio |
| :--------------- | :---------- | :--------------------- |
| Up to 17 pt      | Any         | 4.5:1                  |
| 18 pt and larger | Any         | 3:1                    |
| Any              | Bold        | 3:1                    |

To learn more making text in your app accessible to all users, see [Text Size and Weight](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Technologies/Accessibility/Text%20Size%20and%20Weight).

> 앱의 텍스트에 모든 사용자가 접근할 수 있도록 만드는 방법은 다음 문서를 참조하세요.