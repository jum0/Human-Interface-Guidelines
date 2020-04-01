# Quick Look
Within your app, Quick Look lets people preview Keynote, Numbers, Pages, and PDF documents, as well as images and other types of files, even if your app doesn't support those file formats. Mail uses Quick Look for viewing attachments. After downloading an attachment, Mail shows the attachment’s icon and file name within the message. Tapping the icon displays a preview of the attachment.

> 앱에서, Quick Look은 사용자가 이미지와 앱에서 지원하지 않는 형식의 파일들뿐만 아니라, Keynote, Numbers, Pagaes 및 PDF 문서를 미리 볼 수 있도록 합니다. 메일 앱은 첨부 파일을 확인하기 보기 위해서 Quick Look을 사용합니다. 첨부 파일을 다운로드한 후, 메일 앱은 메시지 안에서 첨부 파일의 아이콘, 파일 이름을 보여줍니다. 아이콘을 탭 하면 첨부 파일의 미리 보기를 보여줍니다.



<img width="545" alt="스크린샷 2020-04-01 오후 9 40 38" src="https://user-images.githubusercontent.com/40762111/78138182-7e6ddb80-7461-11ea-86c1-d19cde5862ba.png">



**Present previews appropriately for the current context.** On iPhone, if your app has a navigation bar, slide the preview into place like any other view in your app’s hierarchy. On iPads, or if your app doesn’t have its own navigation bar, open the preview in a full-screen modal view that includes a navigation bar. With both methods, the navigation bar includes a button for exiting Quick Look, as well as preview-specific buttons for performing actions like sharing and markup. If your app includes a toolbar, any preview-specific buttons appear here instead of in the navigation bar.

> **현재 컨텍스트에서 적절하게 미리 보기를 보여주세요.** 아이폰에서 내비게이션 바가 있다면, 앱의 계층의 다른 부와 같이 미리 보기를 밀어 넣으세요. 아이패드에서 또는 내비게이션 바가 없다면, 내비게이션 바를 포함한 전체 화면 모델 뷰 안에서 미리 보기를 켜세요. 두 가지 방법으로, 내비게이션 바는 공유하기와 마크업과 같은 동작을 수행하는 구체적인 미리 보기 버튼뿐만 아니라 Quick Look을 벗어나는 버튼을 포함합니다. 툴바를 포함한다면, 구체적인 미리 보기 버튼이 내비게이션 바보다는 여기에 나타난다.

For developer guidance, see [Document Interaction Programming Topics for iOS](https://developer.apple.com/library/content/documentation/FileManagement/Conceptual/DocumentInteraction_TopicsForIOS/Introduction/Introduction.html) and [Quick Look](https://developer.apple.com/documentation/quicklook).

> 개발자 가이드는, 다음 문서를 확인하세요.