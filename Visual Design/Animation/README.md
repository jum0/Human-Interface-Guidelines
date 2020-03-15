# Animation
Beautiful, subtle animation throughout iOS builds a visual sense of connection between people and content onscreen. When used appropriately, animation can convey status, provide feedback, enhance the sense of direct manipulation, and help users visualize the results of their actions.

> iOS 전체에 걸친 아름답고 절묘한 애니메이션은 사용자와 화면 속의 콘텐츠 사이에 시각적인 연결성을 만들어줍니다. 적절하게 사용될 때, 애니메이션은 상태를 전달할 수 있고, 피드백을 제공할 수 있으며, 직접적인 조작감을 향상시키고 사용자이 조작하는 결과를 시각화할 수 있도록 도와줍니다.

<img width="279" alt="스크린샷 2020-03-15 오후 9 29 37" src="https://user-images.githubusercontent.com/40762111/76701405-354d2600-6704-11ea-8377-64b8e87b7ebc.png">

> [See example](https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/animation/)



**Use animation and motion effects judiciously.** Don’t use animation for the sake of using animation. Excessive or gratuitous animation can make people feel disconnected or distracted, especially in apps that don’t provide an immersive experience. iOS uses motion effects, such as a parallax effect, to create the perception of depth on the Home screen and in other areas. These effects can increase understanding and enjoyment, but overusing them can make an app feel disorienting and difficult to control. If you implement motion effects, always test the results to make sure they work well.

> **애니메이션과 모션 효과를 분별하여 사용하세요.** 애니메이션을 사용하기 위한 애니메이션은 사용하지 마세요. 지나치거나 불필요한 애니메이션은 사용자가 연결성을 저하시키거나 산만하게 만들어, 특히 앱에서 몰입할 수 있는 경험을 제공하지 못합니다. iOS는 시차 효과와 같은 모션 효과를 사용하여 홈 화면과 다른 장소의 깊이를 만들어냅니다. 이러한 효과들은 이해와 즐거움을 높이지만, 과도한 사용은 사용자가 앱에서 방향을 잃으며 제어하기 어렵게 만들 수 있습니다. 모션 효과를 넣는다면, 항상 잘 작동하는지 확인하기 위해서 결과를 테스트하세요.



**Strive for realism and credibility.** People tend to accept artistic license, but they can feel disoriented when movement doesn’t make sense or appears to defy physical laws. If someone reveals a view by sliding it down from the top of the screen, for example, they should be able dismiss the view by sliding it back up.

> **사실성과 신뢰성을 얻으려고 노력하세요.** 사용자는 예술적인 허용을 인정하지만, 움직임이 어색하거나 물리적인 법칙을 따르지 않는 것처럼 보일 때 혼란을 느낄 수 있습니다. 예를 들어, 누군가 화면을 스크린 상단에서 아래로 밀어 뷰를 드러내면, 뷰를 다시 위로 올려 보이지 않게 할 수 있어야 합니다.



**Use consistent animation.** A familiar, flowing experience keeps users engaged. They're accustomed to the subtle animation used throughout iOS, such as smooth transitions, fluid changes in device orientation, and physics-based scrolling. Unless you’re creating an immersive experience, such as a game, custom animation should be comparable to the built-in animations.

> **일관성 있는 애니메이션을 사용하세요.** 친숙하고 흐르는 듯한 경험은 사용자의 관심을 유지합니다. 사용자들은 부드러운 전환, 기기 방향의 흐르는 듯한 변화와 물리에 기반한 scrolling과 같이 iOS 전반에 사용되는 절묘한 애니메이션에 익숙합니다. 게임과 같은 경우에서 몰입할 수 있는 경험을 만들 수 없다면, 커스텀 애니메이션은 기본 애니메이션과  비교할 수 있는 수준으로 되어야 합니다.



**Make animations optional.** When the option to reduce motion is enabled in accessibility preferences, your app should minimize or eliminate application animations. For guidance, see [Motion](https://developer.apple.com/design/human-interface-guidelines/accessibility/overview/appearance-effects/#motion).

> **애니메이션을 선택할 수 있도록 만드세요.** 접근성 설정에서 모션을 줄이는 옵션이 사용된다면, 앱은 사용되는 애니메이션을 최소화하거나 줄여야 합니다. 자세한 가이드는 다음 문서를 참조하세요.