# Loading

When content is loading, a blank or static screen can make it seem like your app is frozen, resulting in confusion and frustration, and potentially causing people to leave your app.

> 콘텐츠가 로딩 중일 떄, 아무것도 나타내지 않는 화면이나 움직이지 않는 화면은 앱이 멈춰있는 듯한 느낌을 주어, 결과적으로 혼란을 야기할 수 있습니다 그리고 잠재적으로 사용자가 앱에서 떠나게 만들 수도 있습니다.

<img width="285" alt="스크린샷 2020-03-01 오후 8 49 06" src="https://user-images.githubusercontent.com/40762111/75625120-51c66a00-5bfe-11ea-9f85-f58fd6cdbbf8.png">

**Make it clear when loading is occurring.** At minimum, show an activity spinner that communicates something is happening. Even better, display explicit progress so people can gauge how long they’ll be waiting.

> **로딩 중일 때 명확하게 하세요.** 최소한, 무언가가 진행 중이라는 것을 나타내는 activity spinner를 보여주세요. 명확한 progress를 사용해서 사용자가 얼마나 더 기다려야 하는지 알 수 있도록 보여주는 것은 더 좋습니다.



**Show content as soon as possible.** Don’t make people wait for content to load before seeing the screen they're expecting. Show the screen immediately, and use placeholder text, graphics, or animations to identify where content isn't available yet. Replace these placeholder elements as the content loads. Whenever possible, preload upcoming content in the background, such as while an animation is playing or the user is navigating a level or menu.

> **가능한 한 빨리 콘텐츠를 보여주세요.** 사용자가 예상하는 화면을 보기 전에 사용자가 콘텐츠가 로드되는 것을 기다리게 하지 마세요. 화면을 즉시 보여주고, placeholder text, graphics 또는 animations을 사용해서 어떤 콘텐츠가 아직 나타나지 않았는지 알 수 있도록 하세요. 이러한 placeholder 요소들은 콘텐츠가 나타나면 변경하세요. Animation이 재생되거나, 사용자가 level 또는 menu를 둘러보는 동안 등, 가능한 백그라운드에서 다음 콘텐츠를 미리 로드하세요.



**Educate or entertain people to mask loading time.** Consider showing hints about gameplay, entertaining video sequences, or interesting placeholder graphics.

> **로딩 시간을 숨기기 위해서 사용자에게 무엇을 알려주거나, 그들을 즐겁게 하세요.** 게임을 할 때 도움이 되는 힌트를 보여주는 것, 비디오 sequences, 또는 흥미로운 placeholder graphics로 즐겁게 하는 것을 고려하세요.

<img width="558" alt="스크린샷 2020-03-01 오후 8 50 27" src="https://user-images.githubusercontent.com/40762111/75625124-5428c400-5bfe-11ea-8fe2-c17689476768.png">

> [See example](https://developer.apple.com/design/human-interface-guidelines/ios/app-architecture/loading/)



**Customize loading screens.** Although standard progress indicators are usually OK, they can sometimes feel out of context. Consider designing a more immersive experience through custom animations and elements that match the style of your app or game.

> **로딩 화면을 마음대로 꾸며 보세요.** 기본적인 progress indicators가 보통 괜찮지만, 사용자들은 때때로 context와 어울리지 않는다고 느낄 수 있습니다. 앱이나 게임의 스타일에 적합한 custom animations와 요소로 더 몰입할 수 있는 경험을 제공해보세요.



For additional guidance, see [Progress Indicators](https://developer.apple.com/design/human-interface-guidelines/ios/controls/progress-indicators/).

> 추가적인 가이드 라인은 다음 문서를 확인하세요.