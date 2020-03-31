# Sharing and Actions
Share extensions provide a convenient way to share information from the current context with apps, social media accounts, and other services. Action extensions let people initiate content-specific tasks, such as adding a bookmark, copying a link, or saving an image. People access share extensions and action extensions by tapping an Action button in an app to display an activity view. An activity view shows only extensions relevant to the current context. You wouldn’t see text manipulation actions while editing a video, for example. Within an activity view, share extensions are listed above action extensions.

> 공유 더 보기는 앱의 현재 컨텍스트, 소셜 미디어 계정 및 다른 서비스로부터 정보를 공유하는 편리한 방법을 제공합니다. Action 더 보기는 사용자가 북마크를 추가하거나, 링크를 복사하는 것 또는 이미지를 저장하는 것과 같은 구체적인 콘텐츠 작업을 시작할 수 있도록 합니다. 사용자들은 activity 뷰를 보여주기 위해서 Action 버튼을 탭 하여 공유 더 보기와 action 더 보기에 접근합니다. Activity 뷰는 오직 현재 컨텍스트와 관련된 더 보기만을 보여줍니다. 예를 들어, 비디오를 편집하는 동안에는 텍스트 변경 action을 볼 수 없습니다. Activity 뷰 내에서, 공유 더 보기는 action 더 보기 위에 나열됩니다.

<img width="274" alt="스크린샷 2020-03-31 오후 2 17 21" src="https://user-images.githubusercontent.com/40762111/77989706-6a8b8200-735a-11ea-8b9c-8891ca17beb2.png">

**Enable a single, focused task.** An extension isn’t a mini-app. It performs a narrowly scoped task related to the current context.

> **하나의, 집중된 동작을 실행하세요.** 더 보기는 작은 앱이 아닙니다. 현재 컨텍스트와 관련된 좁은 범위의 작업을 수행합니다.



**Craft a familiar interface.** For share extensions, the system-provided composition view is familiar and provides a consistent sharing experience throughout the system. Use it whenever possible. For action extensions, include your app name, or design an interface that’s recognizable and feels like a natural extension of your app.

> **친숙한 인터페이스를 만드세요.** 공유 더 보기는, 시스템이 제공하는 구성 뷰는 친숙하고 시스템 전체적으로 일관된 공유하는 경험을 제공합니다. 언제든 가능하다면, 사용하세요. Action 더 보기는, 앱 이름을 포함하거나 인식 가능하고 자연스럽게 앱의 확장처럼 느껴지는 인터페이스를 디자인하세요.



**Streamline and limit interaction.** The best extensions let people perform a task in just a few steps. For example, a share extension might immediately post an image to a social media account with a single tap. Only provide an interface when necessary.

> **인터랙션을 간소화하고 제한을 두세요.** 가장 좋은 확장은 사용자가 단 몇 가지로 작업을 수행하도록 하는 것입니다. 예를 들어, 공유 확장은 하나의 탭으로 즉시 이미지를 소셜 미디어 계정에 게시할 수 있습니다. 필요한 경우에만, 인터페이스를 제공하세요.



**Avoid placing modal views above your extension.** Extensions are displayed within a modal view by default. While an alert might make sense above an extension, avoid layering additional modal views.

> **확장 위에 모델 뷰 배치하는 것은 피하세요.** 확장은 기본적으로 모델 뷰 안에서 보입니다. Alert가 확장 위에 표시될 수 있지만, 추가적인 모달 뷰의 계층화는 피하세요.



**Use your main app to denote the progress of lengthy operations.** An activity view should dismiss immediately after initiating sharing or an action. Time-consuming tasks should continue in the background, and your main app should provide some way to check the status of these tasks. Don’t use notifications for this. People don’t want to see a notification every time a task completes, although it’s fine to notify them if there’s a problem.

> **주 앱을 사용하여 장시간 작업의 진행 상황을 표시하세요.** Activity 뷰는 sharing 또는 action을 시작한 후, 즉시 사라져야 합니다. 시간을 소비하는 작업은 백그라운드에서 진행되어야 하며, 주 앱에서는 이러한 작업들의 상태를 확인하는 몇 가지 방법을 제공해야 합니다. 알림을 사용하지는 마세요. 문제가 있다면 알림을 하는 것을 괜찮지만, 사용자는 작업이 완료될 때마다 알림을 보고 싶어 하지 않습니다.



**Use a template image for an action extension icon.** A template image uses a mask to create an icon. Use black and white with appropriate transparency and antialiasing, and don’t include a drop shadow. Template images should be centered in an area measuring about 70px × 70px.

> Action 확장 아이콘으로 템플릿 이미지를 사용하세요. 템플릿 이미지는 아이콘을 사용하기 위해서 마스크를 사용합니다. 적절한 투명도와 에릴리어싱 제거와 함께 검은색과 흰색을 사용하고, drop shadow를 포함하지 마세요. 템플릿 이미지는 약 70px * 70px 면적을 중심으로 해야 합니다.



For additional guidelines, see [Activity Views](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Views/Activity%20Views). For developer guidance, see [Share](https://developer.apple.com/library/content/documentation/General/Conceptual/ExtensibilityPG/Share.html) and [Action](https://developer.apple.com/library/content/documentation/General/Conceptual/ExtensibilityPG/Action.html) in [App Extension Programming Guide](https://developer.apple.com/library/content/documentation/General/Conceptual/ExtensibilityPG/index.html).

> 추가적인 가이드는 다음 문서를 확인하세요. 개발자 가이드는 다음 문서를 확인하세요.



**TIP**

Share extensions automatically use your app icon, instilling confidence that the extension is in fact provided by your app.

> 공유 확장은 앱 아이콘을 자동으로 사용하여, 실제로 앱에서 확장이 제공된다는 확신을 심어줍니다.