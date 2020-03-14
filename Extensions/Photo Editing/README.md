# Photo Editing
Photo editing extensions let people modify photos and videos within the Photos app by applying filters or making other changes. Edits are always saved in the Photos app as new files, safely preserving the original versions.

> 사진 편집 확장자는 사용자가 사진 앱에서 필터를 적용하거나 다른 변화를 주어 사진과 영상을 편집할 수 있도록 도와줍니다. 편집은 항상 사진 앱에 새로운 파일로 저장되고, 원본은 안전하게 유지됩니다.

<img width="399" alt="스크린샷 2020-03-14 오후 4 57 50" src="https://user-images.githubusercontent.com/40762111/76677716-0ad06f80-6615-11ea-97e0-517d2fc47596.png">

To access a photo editing extension, a photo must be in edit mode. While in edit mode, tapping the extension icon in the toolbar displays an action menu of available editing extensions. Selecting one displays the extension’s interface in a modal view containing a navigation bar. Dismissing this view confirms and saves the edit, or cancels it and returns to the Photos app.

> 사진 편집 확장자에 접근하기 위해서, 사진은 편집 모드에 있어야만 합니다. 편집 모드에서, 툴바의 확장 아이콘을 탭 하면 사용 가능한 편집 확장 작업 메뉴가 표시됩니다. 하나를 선택하면 내비게이션 바를 포함한 모달 뷰에 확장의 인터페이스가 표시됩니다. 변경하는 것을 그만하면 편집을 확인하고 저장하며, 또는 취소하여 사진 앱으로 돌아갑니다.



**Confirm cancellation of edits.** Editing a photo or video can be time consuming. If someone taps the Cancel button, don’t immediately discard their changes. Ask them to confirm that they really want to cancel, and inform them that any edits will be lost after cancellation. There’s no need to show this confirmation if no edits have been made yet.

> **편집된 것의 취소를 확인하세요.** 사진이나 영상을 편집하는 것은 시간을 소비할 수 있습니다. 누군가 취소 버튼을 눌렀을 때, 편집된 것을 바로 무시하지 마세요. 사용자가 정말 취소하는 것을 원하냐고 물어보고, 취소 후에 변경된 것들이 모두 사라진다는 것을 알려주세요. 편집된 부분이 아직 없다면, 이러한 확인을 보여주는 것이 필요하지 않습니다.



**Don’t provide a custom navigation bar.** Your extension loads within a modal view that already includes a navigation bar. Providing a second navigation bar is confusing and takes space away from the content being edited.

> **커스텀 내비게이션 바를 제공하지 마세요.** 모달 뷰 내에서 로드되는 확장은 이미 내비게이션 바를 포함하고 있습니다. 두 번째 내비게이션 바를 제공하는 것은 사용자를 혼란스럽게 하고, 콘텐츠가 편집될 수 있는 공간을 빼앗게 됩니다.



**Let people preview edits.** It’s hard to approve an edit if you can’t see what it looks like. Let people see the result of their work before closing your extension and returning to the Photos app.

> **사용자가 편집된 것을 미리 확인할 수 있도록 하세요.** 편집된 내용을 볼 수 없다면 넘어가는 것은 어렵습니다. 사용자가 편집을 종료하고 사진 앱으로 돌아가기 전에, 작업의 결과를 보여주세요.



**Use your app icon for your photo editing extension icon.** This instills confidence that the extension is in fact provided by your app.

> **사진 편집 확장 아이콘으로 커스텀 된 아이콘을 사용하세요.** 이것은 편집 확장이 앱에서 제공된다는 사실로 용기를 용기를 북돋우어 줍니다.



For developer guidance, see [Photo Editing](https://developer.apple.com/library/content/documentation/General/Conceptual/ExtensibilityPG/Photos.html) in [App Extension Programming Guide](https://developer.apple.com/library/content/documentation/General/Conceptual/ExtensibilityPG/index.html).

> 개발자 가이드는 다음 문서를 확인하세요.