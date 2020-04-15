# Materials
iOS provides *materials* (or blur effects) that create a translucent effect you can use to evoke a sense of depth. The effect of a material lets views and controls hint at background content without distracting from foreground content. To produce this effect, materials allow background color information to pass through foreground views, while also blurring the background context to maintain legibility.

> iOS는 깊이감을 불러일으키기 위해서 사용할 수 있는 반투명 효과의 materials (또는 블러 효과)를 제공합니다. Material의 효과는 전경 콘텐츠에서 배경 콘텐츠에 주의를 뺏기지 않으며 살짝 비치는 내용들을 보고 제어할 수 있도록 합니다. 이런 효과를 내기 위해서, materials는 배경색 정보가 전경 뷰를 통과하도록 하는 동시에 배경 컨텍스트를 흐리게 하여 가독성을 유지합니다.

When you use the system-defined materials, your elements look great in every context, because these effects automatically adapt to the system’s light and dark modes.

> 시스템에서 정의된 materials를 사용할 때, 요소들은 모든 컨텍스트에서 좋아 보이는데 이런 효과들이 자동으로 시스템의 라이트 및 다크 모드에 맞춰지기 때문입니다.

**TIP**

Materials require the presence of a visual effect view in your view hierarchy. For developer guidance, see [UIVisualEffectView](https://developer.apple.com/documentation/uikit/uivisualeffectview).

> Materials는 뷰 계층에서 visual effect view가 있어야 합니다. UIVisualEffectView와 관련된 가이드는 다음 문서를 참조하세요.

**Be guided by the materials the system uses.** Whenever possible, compare your custom views to system-provided views that enable similar functionality and use the same materials.

> **시스템에서 사용하는 materials의 안내를 받으세요.** 가능하면, 비슷한 기능을 제공하는 시스템 지원 뷰와 커스텀 뷰를 비교하고, 같은 materials를 사용하세요.

**Take advantage of the system-provided colors for text, fills, glyphs, and separators.** The system-provided colors automatically make these items look great on translucent backgrounds. For guidance, see [Dynamic System Colors](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Visual Design/Color).

> **텍스트, 채우기, 아이콘 및 구분자에 관해 시스템에서 제공하는 색상을 활용하세요.** 시스템에서 제공하는 색상은 자동으로 이러한 아이템들을 반투명한 배경에서 좋아 보이도록 합니다. Dynamic System Colors와 관련된 가이드는 다음 문서를 참조하세요.

**When possible, use SF Symbols.** When you use dynamic system colors to color a symbol, or apply a vibrancy effect to it, the symbol looks great in any context. In contrast, full-color images may not have sufficient contrast with the background and may seem out of place when used in a view with a translucent background. For related guidance, see [SF Symbols](https://developer.apple.com/design/human-interface-guidelines/sf-symbols/).

> **가능하면, SF Symbols을 사용하세요.** Symbol을 색칠하거나 생동감 효과(vibrancy effect; contentView 내의 content가 생생하게 보이도록 하는 효과)를 적용하기 위해서 dynamic system color를 사용할 때, symbol은 어떤 컨텍스트에서든 좋아 보입니다. 대조적으로, 전체가 색으로 구성된 이미지는 배경과 충분한 대비를 가지지 못할 수 있고, 반투명 배경의 뷰에서 사용될 때 맞지 않는 것처럼 보일 수도 있습니다. SF Symbols와 관련된 가이드는 다음 문서를 참조하세요.

### System-Defined Materials and Vibrancy

iOS defines materials you can use in specific areas to control the visual separation between the foreground content and the background appearance. The system-provided materials include both light and dark variants that work well against most backgrounds.

> iOS는 전경 콘텐츠와 배경 사이에 시각적인 분리를 조절하기 위해 특정 영역에서 사용할 수 있는 materials를 정의합니다. 시스템에서 제공하는 materials는 대부분의 배경에서 기능을 잘 하는 라이트 및 다크 버전을 포함합니다.

For use in content containers, iOS 13 defines four materials that have different levels of translucency (each material also includes a dark variant):

> 콘텐츠 컨테이너에서 사용하기 위해서, iOS 13은 각기 다른 반투명의 단계를 지닌 네 가지 materials를 정의합니다. (각각의 material은 다크 버전도 포함합니다.)

- [SystemUltraThinMaterial](https://developer.apple.com/documentation/uikit/uiblureffect/style/systemultrathinmaterial)
- [SystemThinMaterial](https://developer.apple.com/documentation/uikit/uiblureffect/style/systemthinmaterial)
- [SystemMaterial](https://developer.apple.com/documentation/uikit/uiblureffect/style/systemmaterial) (default)
- [SystemThickMaterial](https://developer.apple.com/documentation/uikit/uiblureffect/style/systemthickmaterial)

**Consider contrast and visual separation when choosing a material.** There’s no absolute rule for choosing a material to combine with vibrancy effects. As you’re making this choice, consider that:

> **Material을 선택할 때, 대비와 시각적인 분리를 고려하세요.** 생동감 효과와 같이 사용하기 위해 선택하는 material에 절대적인 기준은 없습니다. 선택할 때, 다음 사항을 고려하세요.

- Thicker materials can provide better contrast for text and other elements with fine features

  > 더 두꺼운 materials는 미세한 특징을 지닌 텍스트와 다른 요소들에 더 강한 대비를 제공합니다.

- Translucency can help people retain their context by providing a visible reminder of the content that’s in the background

  > 반투명은 배경에 있는 콘텐츠를 시각적으로 상기시켜줌으로써 사용자가 컨텍스트를 유지할 수 있도록 돕습니다.

iOS 13 also defines vibrancy values for labels, fills, and separators that are specifically designed to work with each material. Vibrancy brightens or darkens UI elements by sampling background colors and modifying saturation and value. Vibrant UI elements integrate better with materials and enhance the translucent effect.

> iOS 13은 또한 각 material과 함께 기능하도록 특별히 설계된 레이블, 채우기 및 구분자에 대한 생동감 효과를 정의합니다. 생동감은 배경 색으로부터 추출하고 채도와 값을 변경함으로써 UI 요소들을 밝게하거나 어둡게 합니다. 생생한 UI 요소들은 materials와 더 잘 어울리고 반투명 효과를 향상시킵니다.

Labels and fills each provide several levels of vibrancy; separators have one level. The names of the levels indicate the relative amount of contrast between an element and the background: the default level has the highest contrast, whereas quaternary (when it exists) has the lowest contrast.

> 레이블과 채우기는 각각 여러 가지 단계의 생동감을 제공합니다; 구분자은 한 가지 단계를 가지고 있습니다. 이러한 단계들의 이름은 요소와 배경 사이 간 상대적인 대비의 정도를 나타냅니다: 기본 단계는 가장 높은 대비를 지니는 반면에, 네 번째(존재하고 있다면)는 가장 낮은 대비를 지닙니다. 

Except for quaternary, you can use the following vibrancy values for labels on any material. It's not recommended to use quaternary on thin and ultra thin materials, because the contrast is too low.

> 네 번째를 제외하고, 모든 material의 레이블에 다음과 같은 생동감 값을 사용할 수 있습니다. 대비가 너무 낮기 때문에, thin과 ultra thin material에 네 번째를 사용하는 것은 추천하지 않습니다.

- [label](https://developer.apple.com/documentation/uikit/uivibrancyeffectstyle/label) (default)
- [secondaryLabel](https://developer.apple.com/documentation/uikit/uivibrancyeffectstyle/secondarylabel)
- [tertiaryLabel](https://developer.apple.com/documentation/uikit/uivibrancyeffectstyle/tertiarylabel)
- [quaternaryLabel](https://developer.apple.com/documentation/uikit/uivibrancyeffectstyle/quaternarylabel)

You can use the following vibrancy values for fills on all materials.

> 모든 materials의 채우기에서 생동감 값을 사용할 수 있습니다.

- [fill](https://developer.apple.com/documentation/uikit/uivibrancyeffectstyle/fill) (default)
- [secondaryFill](https://developer.apple.com/documentation/uikit/uivibrancyeffectstyle/secondaryfill)
- [tertiaryFill](https://developer.apple.com/documentation/uikit/uivibrancyeffectstyle/tertiaryfill)

iOS defines a single, default vibrancy value for separators ([separator](https://developer.apple.com/documentation/uikit/uivibrancyeffectstyle/separator)) that works well on all materials.

> iOS는 모든 materials에 잘 작동하는 구분자에 하나의 기본 생동감 값을 정의합니다.

**Choose a vibrancy effect based on its semantic meaning.** Avoid mixing these effects; for example, don’t use a label effect for a separator.

> **의미적인 뜻에 기반해서 생동감 효과를 선택하세요.** 예를 들어, 이런 효과들이 중첩되는 것을 피하세요; 구분자에는 레이블 효과를 사용하지 마세요.