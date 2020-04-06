# Dark Mode
In iOS 13.0 and later, people can choose to adopt a dark system-wide appearance called Dark Mode. In Dark Mode, the system uses a darker color palette for all screens, views, menus, and controls, and it uses more vibrancy to make foreground content stand out against the darker backgrounds. Dark Mode supports all accessibility features.

> iOS 13.0 및 그 이상의 버전에서, 사용자들은 다크 모드라고 불리는 시스템 전반의 어두운 모습을 채택하는 것을 선택할 수 있습니다. 다크 모드에서, 시스템은 모든 화면, 뷰, 메뉴 및 컨트롤에서 더 어두운색 팔레트를 사용하고, 더 많은 vibrancy을 사용하여 어두운 배경과 대비하여 앞 쪽의 콘텐츠가 강조되도록 합니다. 다크 모드는 모든 접근성 특징들을 지원합니다.

<img width="546" alt="스크린샷 2020-04-06 오후 12 46 22" src="https://user-images.githubusercontent.com/40762111/78521415-bc258800-7804-11ea-9a99-9e5082ccc809.png">

In Settings, people can choose Dark Mode as their default interface style and schedule automatic changes between the appearance modes. Because people make these choices at a systemwide level, they generally expect all apps to respect their preferences.

> 설정에서, 사용자들은 다크 모드를 기본 인터페이스 스타일로 설정할 수 있고, appearance 모드가 자동적으로 변하게 계획할 수 있습니다. 사용자들은 시스템의 수준에서 설정하기 때문에, 일반적으로 모든 앱들이 그들의 선호하는 대로 적용되는 것을 기대합니다.



**Comply with the appearance mode people choose in Settings.** If you offer an app-specific appearance mode option, you create more work for people because they have to adjust more than one setting. Worse, they may think your app is broken because it doesn't respond to their systemwide appearance choice.

> **사용자가 설정에서 선택하는 appearance 모드를 따르세요.** 애플리케이션 별로 appearance 모드 옵션을 제공하면, 두 개 이상의 설정을 조정해야 하기 때문에 사용자를 위한 더 많은 작업을 만들 수 있습니다. 더 나쁜 것은, 그들이 선택한 시스템 appearance 모드와 다를 수 있기 때문에 앱이 잘못되었다고 생각할 수도 있습니다.



**Test your designs in both light and dark appearances.** See how your interface looks in both appearances, and adjust your designs as needed to accommodate each one. Designs that work well in one appearance might not work in the other.

> **라이트 모드와 다므 모드 모두에서 앱의 디자인을 확인해보세요.** 각각의 모드에서 인터페이스가 어떻게 보이는지 확인하고, 각각의 모드에서 필요한 대로 디자인을 조정하세요. 한 쪽의 모드에서 적합한 디자인이 다른 쪽에서는 아닐 수 있습니다.



**Ensure that your content remains comfortably legible in Dark Mode when you adjust the contrast and transparency accessibility settings.** In Dark Mode, you should test your content with Increase Contrast and Reduce Transparency turned on, both separately and together. You may find places where dark text is less legible when it’s on a dark background. You might also find that turning on Increase Contrast in Dark Mode can result in reduced visual contrast between dark text and a dark background. Although people with strong vision might still be able to read lower contrast text, such text could be illegible for people with visual impairments. For guidance, see [Color and Contrast](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Technologies/Accessibility/Color%20and%20Contrast).

> **접근성 설정에서 색의 대비와 투명도를 조절할 때, 다크 모드에서 콘텐츠를 편하게 읽을 수 있도록 유지하세요.** 다크 모드에서, 대비 상승과 투명도 하락을 각각 및 동시에 실행했을 때의 콘텐츠를 확인해야만 합니다. 어두운 배경이 있을 때, 어두운 텍스트가 읽기 어려워지는 공간을 찾을 수 있습니다. 또한 다크 모드에서 대비 상승을 켰을 때, 어두운 텍스트와 어두운 배경 사이에 시각적인 대비가 낮아지는 결과를 확인할 수도 있습니다. 시력이 좋은 사용자들은 색의 대비가 낮은 텍스트도 잘 읽을 수 있지만, 시각 장애가 있는 사용자들 읽기 힘들 수 있습니다. 가이드는 다음 문서를 참조하세요.



### Dark Mode Colors

The color palette in Dark Mode includes darker background colors and lighter foreground colors that are carefully selected to ensure contrast while maintaining a consistent feel between modes and across apps.

> 다크 모드에서 색상 팔레트는 모드와 앱 간의 일관된 느낌을 유지하면서 색의 대비를 보장하기 위해서 더 어두운 배경색과 더 밝은 전경 색을 포함합니다.



In Dark Mode, the system uses two sets of background colors — called *base* and *elevated* — to enhance the perception of depth when one dark interface is layered above another. The base colors are darker, making background interfaces appear to recede, and the elevated colors are lighter, making foreground interfaces appear to advance.

> 다크 모드에서, 시스템은 base와 elevated라고 불리는 두 가지 종류의 배경 색을 사용해서 어두운 인터페이스가 다른 하나에 씌워졌을 떄 깊이감을 향상시킵니다. 인터페이스를 더 멀어지는 듯하게 만드는  base 색들은 더 어둡고, 전경의 인터페이스를 더 나오는 듯하게 만드는 elevated 색들은 더 밝습니다.



**Prefer the system background colors.** Dark Mode is dynamic, which means that the background color automatically changes from base to elevated when an interface is in the foreground, such as a popover or modal sheet. The system also uses the elevated background color to provide visual separation between apps in a multitasking environment and between windows in a multiple-window context. Using a custom background color can make it harder for people to perceive these system-provided visual distinctions.

> **시스템 배경색을 선호하세요.** 다크 모드는 팝 오버 또는 모달 시트와 같이 인터페이스가 전경에 있을 때 배경색을 자동으로 base에서 elevated로 변경하듯이 역동적입니다. 시스템은 또한 멀티태스킹 환경의 앱 사이에 또는 다중 화면 컨텍스트에서 화면 간 시각적인 분리를 위해서 elevated 배경 색을 사용합니다. 커스텀 배경 색을 사용하는 것은 사용자가 이러한 시스템에서 제공하는 시각적인 독특함을 인지하기 어렵게 만들 수 있습니다.



**Use dynamic colors that adapt to the current appearance.** Semantic colors like [separator](https://developer.apple.com/documentation/uikit/uicolor/3173139-separator) automatically adapt to the current appearance (for guidance, see [Dynamic System Colors]([https://github.com/jum0/Human-Interface-Guidelines/tree/master/Visual%20Design/Color](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Visual Design/Color)/#dynamic-system-colors)). When you need a custom color, add a Color Set asset to your app’s asset catalog and specify the light and dark variants of the color so that it can adapt to the current appearance mode. Avoid using hard-coded color values or colors that don’t adapt.

> **현재 appearance에 적응하기 위해서 역동적인 색을 사용하세요.** Separator와 같은 의미적 색채(색상을 지정하면 시스템이 알아서 모드에 따라 적용하는 색)는 자동적으로 현재 appeaarance에 맞게 변경됩니다.(가이드는 다음 문서를 확인하세요.)



<img width="546" alt="스크린샷 2020-04-06 오후 12 46 34" src="https://user-images.githubusercontent.com/40762111/78521418-bdef4b80-7804-11ea-9663-267b1e1104fc.png">



**Ensure sufficient color contrast in all appearances.** Using system-defined colors ensures a proper contrast ratio between your foreground and background content. For custom colors, aim for a contrast ratio of 7:1, especially for smaller text. For guidance, see [Dynamic System Colors](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Visual%20Design/Color).

> **모든 appeaarance에서 충분한 색 대비를 유지하세요.** 시스템 정의된 색을 사용하는 것은 전경과 배경 콘텐츠 간의 적절한 대비율을 보장합니다. 커스텀 색채는, 특히 작은 텍스트에서 대비율 7:1을 목표로 하세요. 자세한 가이드는 다음 문서를 확인하세요.



**Soften the color of white backgrounds.** If you must use a white background for your content in Dark Mode, choose a slightly darker white that prevents the background from glowing against the surrounding dark content.

> **하얀 배경색은 부드럽게 하세요.** 다크 모드에서 콘텐츠에 하얀 배경을 사용해야만 하는 경우, 어두운 콘텐츠 주변에서 밝게 빛나는 배경을 막는 약간 어두운 하얀색을 선택하세요.



For related guidance, see [Color](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Visual%20Design/Color).

> 관련된 가이드는 다음 문서를 참조하세요.



#### Image, Icon, and Symbol Color

The system uses [SF Symbols](https://developer.apple.com/design/human-interface-guidelines/sf-symbols/), which automatically look great in Dark Mode, and full-color images that are optimized for both light and dark appearances.

> 시스템이 사용하는 SF Symbols은 자동적으로 다크 모드에서 보이기 좋게 바뀌고 라이트 및 다크 모드 모두에서 최적화된 full-color 이미지입니다.



**Use SF Symbols wherever possible.** Symbols look great in both appearance modes when you use [dynamic colors](https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/color/#dynamic-system-colors) to tint them or when you add vibrancy.

> **어디든 가능하다면, SF Symbols을 사용하세요.** Symbols는 색을 입히기 위해 동적인 색을 사용할 때 혹은 vibrancy을 넣을 때, 양쪽 모드 둘 다 적합합니다.



**Design individual glyphs for light and dark appearances when necessary.** A glyph that uses a hollow outline in light mode might look better as a solid, filled shape in Dark Mode.

> **필요하다면, 라이트 및 다크 모드에서 각각의 상형 문자를 디자인하세요.** 라이트 모드에서의 아웃 라인이 움푹 꺼진 상형 문자는 다크 모드에서 안쪽이 채워진 것이 더 좋아 보일 수 있습니다.



**Make sure full-color images and icons look good.** Use the same asset if it looks good in both light and dark modes. If an asset looks good in only one mode, modify the asset or create separate light and dark assets. Use asset catalogs to combine your assets into a single, named image.

> **Full-color 이미지와 아이콘은 괜찮아 보이는 것을 기억하세요.** 라이트 모드나 다크 모드에서 잘 보인다면, 같은 asset을 사용하세요. Asset이 한 쪽의 모드에서만 괜찮아 보인다면, asset을 수정하거나, 라이트 모드와 다크 모드의 asset을 따로 만드세요. Asset을 하나로 합치고, 이름을 짓기 위해서 asset catalogs를 사용하세요.



### Materials

Vibrancy can help maintain good contrast of text on darker backgrounds.

> Vibrancy는 더 어더운 배경에서 텍스트의 대비가 잘 나타나도록 유지하는 것을 도와줍니다.



**Use the system-provided label colors for labels.** The primary, secondary, tertiary, and quaternary label colors adapt automatically to light and dark appearances. For related guidance, see [Typography](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Visual%20Design/Typography).

> **Labels로 시스템에서 제공하는 label 색을 사용하세요.** Primary, secondary, tertiary 및 quaternary label 색은 라이트 및 다크 모드에 자동으로 적응합니다. 관련된 가이드는 다음 문서를 참조하세요.



**Use system views to draw text fields and text views.** System views and controls make your app’s text look good on all backgrounds, adjusting automatically for the presence or absence of vibrancy. When possible, use a system-provided view to display text instead of drawing the text yourself. For developer guidance, see [UITextField](https://developer.apple.com/documentation/uikit/uitextfield) and [UITextView](https://developer.apple.com/documentation/uikit/uitextview).

> **텍스트 필드와 텍스트 뷰를 그리기 위해서 시스템 뷰를 사용하세요.** 시스템 뷰와 controls는 vibrancy의 충분 및 부족을 자동으로 조정하여 배경에서 텍스트가 잘 보이도록 도와줍니다. 가능한 한, 텍스트를 보여주기 위해서 직접 그리기보다는 시스템이 제공하는 뷰를 사용하세요. 개발자 가이드는 다음 문서를 확인하세요.



To learn more about the interplay of vibrancy and materials, see [Materials](https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/materials/).

> vibrancy와 materials의 상호작용에 대해서 더 알고 위해서, 다음 문서를 참조하세요.