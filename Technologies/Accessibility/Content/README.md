# Content
Copy, images, audio, and video supply the information that people want from your app. You can help make your content accessible to everyone by striving for simplicity of expression and providing alternative versions of the information.

> 카피, 이미지, 오디오 및 영상은 사용자가 앱에서 원하는 정보를 제공합니다. 표현의 단순성을 위해 노력하고 정보의 다른 버전을 제공함으로써 모든 사람들이 콘텐츠에 접근 가능하도록 도움을 줄 수 있습니다.



### Copy and Images

**Edit copy so that it is simple and clear.** When copy is straightforward, uncomplicated, and free of errors, all users benefit.

> **카피를 간단하고 명확하게 편집하세요.** 카피가 쉽고, 복잡하지 않으며 오류가 없다면 모든 사용자에게 도움이 됩니다.



**Provide alternative descriptions for all images that convey meaning.** If you don't describe the meaningful images in your content, you prevent VoiceOver users from fully experiencing your app. To create a useful description, start by reporting what would be self-explanatory to someone who is able to see the image. Because VoiceOver reads the text surrounding the image and any captions, focus your description on information that's conveyed by the image itself.

> **의미를 전하는 모든 이미지에 대안의 설명을 제공하세요.** 콘텐츠에서 의미를 지닌 이미지를 설명하지 않는다면, 보이스오버 사용자는 앱을 온전히 경험하는 데 어려움을 느낍니다. 유용한 설명을 만들기 위해서, 이미지를 볼 수 있는 사람이 스스로에게 설명할 만한 것을 보고하는 것으로 시작하세요. 보이스오버는 이미지 주변에 있는 텍스트와 캡션들을 읽기 때문에, 설명으로 이미지 그 자체를 전달하는 정보에 초점을 맞추세요.



<img width="483" alt="스크린샷 2020-03-25 오전 10 47 57" src="https://user-images.githubusercontent.com/40762111/77493310-1d08a400-6e86-11ea-95b3-11c9b401fc30.png">



**Make infographics fully accessible.** Provide a concise description of the infographic that explains what it conveys. If people can interact with the infographic to get more or different information, you need to make these interactions available to VoiceOver users, too. The accessibility APIs provide ways to represent custom interactive elements so that assistive technologies can help people use them. For developer guidance, see [UIKit Accessibility](https://developer.apple.com/documentation/uikit/accessibility) and [AppKit Accessibility](https://developer.apple.com/documentation/appkit/accessibility).

> **인포그래픽이 전체적으로 접근 가능하도록 만드세요.** 전달하고자 하는 것을 제시하는 인포그래픽의 간단한 설명을 제공하세요. 사용자가 다양하고 많은 정보를 얻기 위해서 인포그래픽과 의견을 주고받을 수 있다면, 이러한 인터랙션을 보이스오버 사용자도 이용할 수 있도록 만들어야 합니다. 접근성 API는 사용자 정의 요소를 나타내는 방법들을 제공하여 보조 기술이 사용자가 그것들을 사용하는 것을 도울 수 있습니다. 개발자 가이드는 다음 문서를 참조하세요.



**Hide purely decorative images from assistive technologies.** Making VoiceOver describe a purely decorative image can waste time for users and add to their cognitive load without providing any benefit.

> **보조 기술에서 오직 장식을 위한 이미지는 숨기세요.** 보이스오버가 완전히 장식을 위한 이미지를 설명하도록 하는 것은 사용자의 시간을 낭비하고 어떠한 이익도 없이 인지적인 부하를 가중시킬 수 있습니다.



**Give each screen a unique title and provide headings that identify sections in your information hierarchy.** When people arrive on a screen, the title is the first piece of information they receive from an assistive technology. To help people understand the structure of your app, create a unique title for each screen that succinctly describes its contents or purpose. Similarly, people need accurate section headings to help them build a mental map of the information hierarchy of each screen.

> **각각의 화면에 특별한 제목과 주고, 정보 계층에서 섹션을 구분할 수 있는 머리말을 주세요.** 사용자들이 화면에 진입했을 때, 제목은 사용자들이 보조 기술의 도움으로 얻게 되는 첫 번째 정보입니다. 사용자가 앱의 구조를 이해할 수 있도록 돕기 위해서, 각 화면의 콘텐츠와 목적을 간단하게 설명하는 특별한 제목을 구성하세요. 비슷하게, 사용자는 각 화면의 정보 계층의 멘탈 맵 구성을 돕기 위해서 정확한 섹션의 머리말이 필요합니다.



### Audio and Video

**Provide closed captions.** Closed captions give people a textual equivalent for the audible information in a video. Using closed captions lets you provide multiple translations for the same content and allows the system to choose the version that matches the user’s settings. Because closed captions aren't always available, it's important to provide subtitles, too. For developer guidance, see [Adding Subtitles and Alternative Audio Tracks](https://developer.apple.com/documentation/avfoundation/media_assets_playback_and_editing/adding_subtitles_and_alternative_audio_tracks).

> **표시 여부를 사용할 수 있는 자막(CC)을 제공하세요.** CC는 영상에서 사용자에게 원문과 동일한 청각적인 정보를 제공합니다. CC를 사용하는 것은 동일한 콘텐츠에 다양한 해석을 제공하고, 시스템이 사용자의 설정한 버전을 선택할 수 있도록 합니다. CC를 항상 사용할 수 있는 것은 아니기 때문에, 일반 자막을 제공하는 것 또한 중요합니다. 개발자 가이드는 다음 문서를 확인하세요.



**Supply audio descriptions.** Use audio descriptions to provide a spoken narration of important information that is presented only visually.

> **오디오 설명을 제공하세요.** 오디오 설명을 사용하여 시각적으로만 표시되는 중요한 정보의 구술 내레이션을 제공하세요.



**Consider providing transcripts.** It can be a good idea to provide a complete textual description of a video, covering both audible and visual information, so that people can enjoy the video in different ways.

> **대화록 제공을 고려하세요.** 시각 및 청각적인 정보를 아우르는 영상의 완전한 원문의 설명 제공은 좋은 방법이 될 수 있어, 사용자가 다른 방식으로 영상을 즐길 수 있습니다.