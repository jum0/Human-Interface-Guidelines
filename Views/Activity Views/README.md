# Activity Views

An activity is a task, such as Copy, Favorite, or Find, that’s useful in the current context. Once initiated, an activity can perform a task immediately, or ask for more information before proceeding. Activities are managed by an activity view, which appears as a sheet or popover, depending on the device and orientation. Use activities to give people access to custom services or tasks your app can perform.

> Activity는 Copy, Favorite 또는 Find와 같은 작업이며 현재 컨텍스트에서 유용합니다. 일단 시작되면, activity는 작업을 즉시 수행할 수 있고, 진행하기 전에 더 많은 정보를 요구할 수 있습니다. Activities는 기기나 방향에서 따라서 sheet 혹은 popover처럼 보이는 activity view에서 관리됩니다. 사용자가 앱이 수행할 수 있는 커스텀 서비스나 작업들에 접근하도록 activities를 사용하세요.

<img width="274" alt="스크린샷 2020-03-29 오후 6 46 08" src="https://user-images.githubusercontent.com/40762111/77845960-b53bbb80-71ed-11ea-8f27-d5db40556820.png">

The system provides a number of built-in activities, including Print, Message, and AirPlay. These tasks always appear first in activity views and can’t be reordered. You don’t need to create custom activities that perform these built-in tasks. Activity views also display share and action extensions from other apps. See [Sharing and Actions](https://github.com/jum0/Human-Interface-Guidelines/tree/master/Extensions/Sharing%20and%20Actions).

> 시스템은 Print, Message, AirPlay를 포함해서 많은 내장된 activities를 제공합니다. 이러한 작업들은 항상 activity view에서 먼저 나타나고, 다시 제공될 수 없습니다. 이러한 내장된 작업들을 수행하는 커스텀 activities를 만들 필요는 없습니다. Activity views는 또한 다른 앱으로부터의 공유와 추가 동작을 보여줍니다. 다음 문서를 참조하세요.

**Design simple template images to represent your custom activities.** A template image uses a mask to create an icon. Use black and white with appropriate transparency and antialiasing, and don’t include a drop shadow. Template images should be centered in an area measuring about 70px × 70px.

> **커스텀 activities를 나타내기 위해서 간단한 템플릿 이미지를 디자인하세요.** 템플릿 이미지는 마스크를 사용해서 아이콘을 생성합니다. 적절한 투명도와 엘리어싱(컴퓨터 그래픽에서 해상도의 한계로 선 등이 우둘투둘하게 되는 현상)을 사용하고 drop shadow를 포함하지 마세요. 템플릿 이미지는 약 70px * 70px의 공간에서 중심으로 되어야 합니다.



**Craft activity titles that succinctly describe your tasks.** Titles appear below the icons in an activity view. Short titles work best. When a title is too long, iOS first shrinks the text and then—if the title is still too long—truncates it. In general, avoid including your company or product name in a title.

> **작업을 간단하게 설명하는 activity 제목을 공들여 만드세요.** 제목은 activity view에서 아이콘의 아래에 위치합니다. 짧은 제목이 가장 좋습니다. 제목이 너무 길다면, iOS는 먼저 텍스트를 줄이고, 여전히 길다면 ...으로 잘라냅니다. 일반적으로, 제목으로 회사나 제품 이름을 포함하는 것은 피하세요.



**Make sure activities are appropriate for the current context.** Although system-provided tasks can’t be reordered in an activity, they can be excluded if they aren’t applicable to your app. For example, to prevent people from printing images, you can exclude the Print activity. You can also identify which custom tasks to show at any given time.

> **Activities는 현재 컨텍스트에 적합하다는 것을 확인하세요.** 시스템이 제공하는 동작들이 activity에서 다시 제공될 수 없지만, 앱에서 적용되지 않은 동작들은 제외될 수 있습니다. 예를 들어, 사용자가 이미지 프린팅 하는 것을 막기 위해서, Print activity를 제외할 수 있습니다. 또한 특정 시간에 표시할 커스텀 작업들을 식별할 수도 있습니다.



**Use the Action button to display an activity view.** People are accustomed to accessing system-provided activities when they tap the Action button. Avoid confusing people by providing an alternative way to do the same thing.

> **Activity view를 보여주기 위해서 Action 버튼을 사용하세요.** 사용자들은 Action 버튼을 탭 했을 때 시스템이 제공하는 activities에 접근하는 것을 당연하게 생각합니다. 같은 것을 하기 위해 대안을 제공하여 사용자의 혼란을 피하세요.

<img width="274" alt="스크린샷 2020-03-29 오후 6 46 56" src="https://user-images.githubusercontent.com/40762111/77845962-b836ac00-71ed-11ea-9b27-d646a4817d42.png">

For developer guidance, see [UIActivityViewController](https://developer.apple.com/documentation/uikit/uiactivityviewcontroller) and [UIActivity](https://developer.apple.com/documentation/uikit/uiactivity).

> 개발자 가이드는 다음을 참조하세요.