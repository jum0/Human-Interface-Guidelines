# Popovers

A popover is a transient view that appears above other content onscreen when you tap a control or in an area. Typically, a popover includes an arrow pointing to the location from which it emerged. Popovers can be nonmodal or modal. A nonmodal popover is dismissed by tapping another part of the screen or a button on the popover. A modal popover is dismissed by tapping a Cancel or other button on the popover.

> Popover는 control 또는 공간을 탭 했을 때, 화면의 다른 콘텐츠 위에 나타는 일시적인 뷰입니다. 대표적으로, popover는 그것이 나타는 위치를 가리키는 화살표 모양을 가지고 있습니다. Popovers는 modal 형태를 될 수도 있고, 되지 않을 수도 있습니다. Modal이 아닌 형태의 popover는 popover 위의 버튼이나 화면의 다른 부분을 탭 하면 사라지게 됩니다. Modal 형태의 popover는 popover 위의 취소 또는 다른 버튼을 탭 하면 사라지게 됩니다.



Popovers are most appropriate on larger screens and can contain any variety of elements, including navigation bars, toolbars, tab bars, tables, collections, images, maps, and custom views. When a popover is visible, interactions with other views are normally disabled until the popover is dismissed. Use a popover to show options or information related to the content onscreen. Many iPad apps, for example, show a popover of sharing options when you tap the Action button.

> Popovers는 큰 화면에 매우 효과적이고, 내비게이션 바, 툴바, 표, 컬렉션, 이미지, 지도, 커스텀 뷰 등 다양한 요소들을 포함할 수 있습니다. Popover가 나타나면, 일반적으로 다른 뷰와의 인터랙션은 popover가 사라질 때까지 사용할 수 없습니다. 화면 속의 콘텐츠와 관련된 선택지이나 정보를 보여주기 위해서 popover를 사용하세요. 예를 들어, 많은 iPad 앱들은 Action 버튼을 탭 했을 때, 다양하게 이용할 수 있는 옵션들을 보여줍니다.



<img width="547" alt="스크린샷 2020-03-12 오후 5 58 45" src="https://user-images.githubusercontent.com/40762111/76504497-2dcf1800-648b-11ea-98fb-69b96dba9802.png">

**Avoid displaying popovers on iPhones.** Generally, popovers should be reserved for use in iPad apps. In iPhone apps, utilize all available screen space by presenting information in a full-screen modal view, rather than in a popover. For related guidance, see [Modality](https://github.com/jum0/Human-Interface-Guidelines/tree/master/App%20Architecture/Modality).

> **아이폰에서 popovers 보여주는 것을 피하세요.** 일반적으로, popovers는 iPad 앱에서 사용하도록 되어 있습니다. 아이폰 앱에서는, 정보를 popover보다는 전체 화면 modal 뷰로 보여주어 화면의 모든 공간을 이용하세요. 관련된 가이드는 다음 문서를 확인하세요.



**Use a Close button for confirmation and guidance only.** A Close button, such as Cancel or Done, is worth including if it provides clarity, such as exiting with or without saving changes. In general, a popover should close automatically when its presence is no longer necessary. In most cases, a popover should close when someone taps outside of its bounds or selects an item in the popover. If multiple selections can be made, the popover should remain open until someone explicitly dismisses it or taps outside of its bounds.

> **확인과 가이드에서만 닫기(Close) 버튼을 사용하세요.** 취소(Cancel) 또는 완료(Done) 같은 닫기 버튼은 변경 사항을 저장하거나 저장하지 않고 종료하는 것과 같이 명확성을 제공하는 점에서 가치가 있습니다. 일반적으로, popover는 그것의 존재할 필요가 더 이상 없다면 자동적으로 닫혀야 합니다. 많은 경우에서 popoversms는 경계의 바깥 부분을 탭 하거나 popover 내의 아이템을 선택했을 때, 닫혀야 합니다. 여러 개의 선택지들이 있다면, popover는 확실히 그것을 닫거나 popover가 아닌 다른 부분을 탭 할 때까지, 열려 있어야 합니다.



**Always save work when automatically closing a nonmodal popover.** It’s easy to dismiss a nonmodal popover unintentionally by tapping another part of the screen. Discard work only when someone taps an explicit Cancel button.

> **Modal이 아닌 형태의 popover가 자동으로 닫힐 때, 하고 있는 작업을 자동으로 저장하세요.** Modal이 아닌 형태의 popover는 의도치 않게 화면의 다른 부분을 탭 하여 닫히기 쉽습니다. 정확하게 취소 버튼을 탭 했을 때만, 하고 있던 작업을 버리세요.



**Position popovers appropriately onscreen.** A popover’s arrow should point as directly as possible to the element that revealed it. Because popovers can’t be dragged around the screen, a popover shouldn’t cover essential content people may need to see while using the popover. A popover also shouldn’t cover the element that was tapped to show the popover.

> **Popovers를 화면 속에 적절하게 배치하세요.** Popover의 화살표는 가능한 직접적으로 popover를 나타내는 요소를 가리켜야 합니다. 화면 속에서 popovers는 드래그 될 수 없기 때문에, 사용자가 그것을 사용하는 동안에, 사용자에게 필요할 수 있는 필수적인 콘텐츠를 가리지 않도록 해야 합니다. 또한 popover는 popover를 보여주기 위해 탭 되는 요소들을 가리지 않아야 합니다.



**Show one popover at a time.** Displaying multiple popovers clutters the interface and causes confusion. Never show a cascade or hierarchy of popovers, in which one emerges from another. If you need to show a new popover, close the open one first.

> **한 번에 하나의 popover를 보여주세요.** 여러 개의 popovers를 보여주면 인터페이스가 복잡해지고 혼란스러워집니다. 길게 늘여진 popovers나 그것의 계층을 보여주지 말고, 차례로 보여주세요. 새로운 popover를 보여주려고 한다면, 먼저 열린 것을 닫으세요.



**Don’t show another view over a popover.** Except for an alert, nothing should be displayed on top of a popover.

> **Popover에 다른 뷰는 보여주지 마세요. ** 알림을 제외하고, popover 위에 다른 것이 보이지 않도록 하세요.



**When possible, let users close one popover and open another with a single tap.** Avoiding extra taps is especially desirable when several different bar buttons each open a popover.

> **가능하다면, 사용자가 한 번의 탭으로 popover를 닫고 다른 popover를 열 수 있도록 하세요.** 특히 몇 개의 다른 bar 버튼들이 각각 popover를 열 때, 추가적인 탭을 요구하지 않는 것을 바람직합니다.



**Avoid making a popover too big.** A popover shouldn’t take over the entire screen. Make it only big enough to display its contents and point to the place it came from. Be aware that the system might adjust the size of a popover to ensure it fits well onscreen.

> **너무 큰 popover 만드는 것을 피하세요.** Popover는 전체 화면을 차지하지 않도록 해야 합니다. Popover의 콘텐츠를 보여줄 수 있을 만큼의 충분한 크기로 만들고 어디서 나왔는지 가리키도록 하세요. 시스템이 화면에 잘 맞도록 popover의 크기를 조정할 수 있다는 점을 유의하세요.



**Make sure custom popovers look like popovers.** Although you can customize many of the visual aspects of a popover, avoid creating a design people might not recognize as a popover. Popovers tend to work best when they contain standard controls and views.

> **커스텀 popovers가 popovers와 비슷해야 하는 것을 명심하세요.** Popover의 많은 시각적인 부분을 커스텀 할 수 있지만, 사용자가 popover로 인지하지 못할 수 있는 디자인은 피하세요. Popovers는 표준의 controls와 뷰를 가질 때, 가장 효과적인 경향이 있습니다.



**Provide a smooth transition when changing the size of a popover.** Some popovers provide both condensed and expanded views of the same information. If you adjust the size of a popover, animate the change to avoid giving the impression that a new popover replaced the old one.

> **Popover의 크기를 변경할 때는 부드럽게 전환하세요.** 몇몇의 popovers는 같은 정보를 좁은 뷰와 넓은 뷰에 동시에 제공합니다. Popover의 크기를 조정한다면, 새로운 popover가 이전의 popover를 대체한다는 인상을 주지 않기 위해서 변화에 움직이는 효과를 주세요.



For developer guidance, see [UIPopoverPresentationController](https://developer.apple.com/documentation/uikit/uipopoverpresentationcontroller).

> 개발 가이드는 다음 문서를 확인해 주세요.