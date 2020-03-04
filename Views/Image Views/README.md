# Image Views
An image view displays a single image or an animated sequence of images over a transparent or opaque background. Within an image view, images may be stretched, scaled, sized to fit, or pinned to a specific location. Image views are noninteractive by default.

> Image view는 투명하거나 불투명한 배경에 하나의 이미지 또는 애니메이션으로 배열되어 있는 이미지를 보여줍니다. Image view 내에서 늘이거나, 크기를 조정하고 특정 위치에 고정할 수도 있습니다. Image view는 기본적으로 인터랙티브하지는 않습니다.



<img width="276" alt="스크린샷 2020-03-04 오전 11 10 49" src="https://user-images.githubusercontent.com/40762111/75837687-f4eacf80-5e08-11ea-8b68-91335fdf099f.png">

**If possible, make sure all images in an animated sequence are consistently sized.** Ideally, images should be prescaled to fit the view so the system doesn't have to do any scaling. If the system must perform scaling, it's easiest to achieve the desired results when all images are the same size and shape.

> **가능한 한, 애니메이션으로 순서를 지니는 이미지들이 동일한 사이즈를 가지도록 해주세요.** 이상적으로, 이미지들은 view에 맞게 크기를 조정하여 시스템에서 크기를 따로 조정할 필요가 없게 해야 합니다. 시스템에서 크기를 조정해야만 한다면 모든 이미지가 같은 크기와 모양을 가지고 있을 때, 원하는 목표를 가장 쉽게 도달할 수 있습니다.



For developer guidance, see [UIImageView](https://developer.apple.com/documentation/uikit/uiimageview).

> 개발자 가이드는 다음 문서를 확인해 주세요.



**NOTE**

An image that’s been configured as a template image discards its color and adopts any tint that’s been applied to the enclosing image view. See [Custom Icons](https://developer.apple.com/design/human-interface-guidelines/ios/icons-and-images/custom-icons/). For developer guidance, see [UIImageRenderingModeAlwaysTemplate](https://developer.apple.com/documentation/uikit/uiimagerenderingmode/uiimagerenderingmodealwaystemplate) in [UIImage](https://developer.apple.com/documentation/uikit/uiimage).

> 템플릿 이미지로 구성된 이미지는 해당 색상을 무시하고 enclosing image view에 적용된 모든 색상을 채택합니다. 개발자 가이브는 다음 문제를 확인해주세요.