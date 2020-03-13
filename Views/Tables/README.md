# Tables

A table presents data as a scrolling, single-column list of rows that can be divided into sections or groups. Use a table to display large or small amounts of information cleanly and efficiently in the form of a list. Generally speaking, tables are ideal for text-based content, and often appear as a means of navigation on one side of a split view, with related content shown on the opposite side. For guidance, see [Split Views](https://developer.apple.com/design/human-interface-guidelines/ios/views/split-views/).

> 표는 데이터를 sections 혹은 groups에 의해 나누어질 수 있는 행의 하나의 열 목록을 scrolling 하여 나타냅니다. 크고 작은 정보의 양을 목록의 형태로 깔끔하고 효과적으로 보여주기 위해서 표를 사용하세요. 일반적으로 말해서, 표는 텍스트로 된 콘텐츠에 이상적이며, 종종 분할된 뷰의 한 쪽에 내비게이션의 수단으로 나타나고, 반대편에 관련 콘텐츠가 표시됩니다. 가이드는 다음 문서를 확인하세요.



iOS provides three styles of table: plain, grouped, and inset grouped.

> iOS는 plain, grouped, inset grouped의 세 가지 표 스타일을 제공합니다.



**Plain.** Rows can be separated into labeled sections, and an optional index can appear vertically along the right edge of the table. A header can appear before the first item in a section, and a footer can appear after the last item.

> **Plain.** 행은 labeled section으로 구분될 수 있고, 선택적인 색인은 표의 오른쪽 가장 자리를 따라서 수직으로 나타납니다. Header는 section에서 첫 번째 아이템 전에 나타날 수 있고, footer는 마지막 아이템의 후에 나타날 수 있습니다.

<img width="269" alt="1" src="https://user-images.githubusercontent.com/40762111/76538497-be751a80-64c2-11ea-958d-77c210a684c9.png">

**Grouped.** Rows are displayed in groups, which can be preceded by a header and followed by a footer. This style of table always contains at least one group and each group always contains at least one row. A grouped table doesn’t include an index.

> **Grouped.** 행은 header가 선행되고, footer가 따라올 수 있는 groups로 보입니다. 이러한 표의 스타일은 항상 최소 하나의 group을 포함하고 각각의 group은 항상 최소 하나의 행을 포함합니다. Grouped 표는 색인을 포함하지 않습니다.

<img width="269" alt="2" src="https://user-images.githubusercontent.com/40762111/76538503-c03ede00-64c2-11ea-9733-283c723e92ec.png">

**Inset grouped.** Rows are displayed in groups that have rounded corners and are inset from the edges of the parent view (as shown on the right of the image above). This style of table always contains at least one group and each group always contains at least one row and can be preceded by a header and followed by a footer. An inset grouped table doesn’t include an index. The inset grouped style works best in a regular width environment. Because there's less space in a compact environment, an inset grouped table can cause text wrapping, especially when content is localized.

> **Inset grouped.** 행은 둥근 모서리와 상위 뷰의 가장자리로부터 삽입된 groups으로 표시됩니다.(아래 이미지의 오른쪽에 보이는 것처럼). 이런 표의 스타일은 항상 최소 한 개의 group을 포함하며 각각의 group은 항상 최소 한 개의 행을 포함하고, header가 선행되고 footer가 따라올 수 있습니다. Inset grouped 표는 색인을 포함하지 않습니다. Inset grouped 스타일은 가로 방향의 환경에서 가장 알맞습니다. 세로로 된 환경에서는 공간이 적기 때문에, 특히 콘텐츠가 각 지역의 특성에 맞춰졌을 때 inset grouped 표는 텍스트가 압축될 수 있습니다.

<img width="543" alt="3" src="https://user-images.githubusercontent.com/40762111/76538537-cfbe2700-64c2-11ea-85fc-bfdc10c9f8f2.png">

**Think about table width.** Thin tables can cause truncation and wrapping, making them hard to read and scan quickly at a distance. Wide tables can also be difficult to read and scan, and can take away space from content.

> **표의 가로를 생각하세요.** 가는 표는 텍스트가 잘리거나 압축되는 것을 유발할 수 있는데, 읽고 빠르게 훑어보기 어렵게 만듭니다. 넓은 표 또한 읽고 훑어보기 어렵게 만들 수 있고, 콘텐츠로부터 공간을 줄이기 어려울 수 있습니다.



**Begin showing table content quickly.** Don’t wait for extensive table content to load before showing something. Fill onscreen rows with textual data immediately and show more complex data—such as images—as it becomes available. This technique gives people useful information right away and increases the perceived responsiveness of your app. In some cases, showing stale, older data may make sense until fresh, new data arrives.

> **표의 콘텐츠를 빠르게 보여주세요.** 무언가를 보여주기 전에 광범위한 표의 콘텐츠가 로드되는 것을 기다리지 마세요. 즉시 본문의 데이터로 화면 속의 행을 채우고 이미지와 같이 더 복잡한 데이터를 표시하세요. 이러한 기술은 사용자에게 유용한 정보를 바로 전달하고, 앱의 인지된 반응성을 향상시킵니다. 어떤 경우에는 새로운 데이터가 전달될 때까지 오래된 데이터를 보여주는 것이 타당할 수 있습니다.



**Communicate progress as content loads.** If a table’s data takes time to load, show a progress bar or spinning activity indicator to reassure people that your app is still running.

> **콘텐츠가 로드될 때 progress로 의사소통을 하세요.** 표의 데이터가 로드되는 데 시간이 걸린다면, progress bar 또는 돌아가는 activity indicator를 보여주어 사용자에게 앱이 여전히 실행 중이라는 사실로 안심시키세요.



**Keep content fresh.** Consider updating your table’s content regularly to reflect newer data. Just don’t change the scrolling position. Instead, add the content to the beginning or end of the table, and let people scroll to it when they’re ready. Some apps display an indicator when new data has been added, and provide a control for jumping right to it. It’s also a good idea to include a refresh control, so people can manually perform an update at any time. See [Refresh Content Controls](https://developer.apple.com/design/human-interface-guidelines/ios/controls/refresh-content-controls/).

> **콘텐츠를 fresh 하게 유지하세요.** 새로운 데이터를 반영하기 위해서 정기적으로 표의 콘텐츠를 업데이트하세요. 단지 scrolling 위치를 변경하지 말고, 표의 시작과 끝에 콘텐츠를 추가하고 사용자가 준비되었을 때 scroll을 할 수 있도록 하세요. 어떤 앱들은 새로운 데이터가 추가되었을 때 indicator를 보여주고 바로 확인할 수 있도록 control을 제공합니다. 또한 refresh control을 포함하여 사용자가 직접 언제든지 업데이트를 수행할 수 있도록 하는 것도 좋은 방법입니다. 자세한 내용은 다음을 확인하세요.



**Avoid combining an index with table rows containing right-aligned elements.** An index is controlled by performing large swiping gestures. If other interactive elements reside nearby, such as disclosure indicators, it may be difficult to discern the user’s intent when a gesture occurs and the wrong element may be activated.

> **오른쪽으로 정렬된 요소들을 포함하는 표의 행과 색인을 같이 쓰이는 것을 피하세요.** 색인은 큰 swiping 제스처를 수행함으로써 제어됩니다. Disclosure indicators(화살표와 같은 것)와 같은 다른 인터랙티브 요소들이 근처에 있다면, 사용자의 제스처가 발생했을 때 의도를 알아차리기 어렵고, 잘못된 요소가 활성화될 수 있습니다.



For developer guidance, see [UITableView](https://developer.apple.com/documentation/uikit/uitableview).

> 개발자 가이드는 다음 문서를 확인하세요.



### Table Rows

You use standard table cell styles to define how content appears in table rows.

> 어떻게 콘텐츠가 표의 행에 나타나는지 정의하기 위해서 표준의 table cell 스타일을 사용하세요.

<img width="274" alt="4" src="https://user-images.githubusercontent.com/40762111/76539016-88846600-64c3-11ea-9463-57a63c9f150f.png">

**Basic (Default).** An optional image on the left side of the row, followed by a left-aligned title. It’s a good option for displaying items that don’t require supplementary information. For developer guidance, see the [UITableViewCellStyleDefault](https://developer.apple.com/documentation/uikit/uitableviewcellstyle/uitableviewcellstyledefault) constant of [UITableViewCell](https://developer.apple.com/documentation/uikit/uitableviewcell).

> **Basic(기본)** 행의 왼쪽의 선택적인 이미지는 뒤로 왼쪽으로 정렬된 제목이 있습니다. 이것은 추가적인 정보를 필요로 하지 않는 아이템을 보여주기 위한 좋은 방식입니다. 개발자 가이드는 다음 문서를 확인하세요.

<img width="274" alt="5" src="https://user-images.githubusercontent.com/40762111/76539022-8b7f5680-64c3-11ea-95bd-86f1b5923062.png">

**Subtitle.** A left-aligned title on one line and a left-aligned subtitle on the next. This style works well in a table where rows are visually similar. The additional subtitle helps distinguish rows from one another. For developer guidance, see the [UITableViewCellStyleSubtitle](https://developer.apple.com/documentation/uikit/uitableviewcellstyle/uitableviewcellstylesubtitle) constant of [UITableViewCell](https://developer.apple.com/documentation/uikit/uitableviewcell).

> **Subtitle.** 한 줄에 왼쪽으로 정렬된 제목과 다음 줄에 왼쪽으로 정렬된 부제입니다. 이러한 스타일은 행이 시각적으로 비슷할 때 잘 어울립니다. 추가적인 부제는 행을 다른 행과 구분할 수 있는데 도움을 줍니다. 개발자 가이드는 다음 문서를 확인하세요.

<img width="274" alt="6" src="https://user-images.githubusercontent.com/40762111/76539024-8c17ed00-64c3-11ea-9d91-ebf33ec132c1.png">

**Right Detail (Value 1).** A left-aligned title with a right-aligned subtitle on the same line. For developer guidance, see the [UITableViewCellStyleValue1](https://developer.apple.com/documentation/uikit/uitableviewcellstyle/uitableviewcellstylevalue1) constant of [UITableViewCell](https://developer.apple.com/documentation/uikit/uitableviewcell).

> **Right Detail (Value 1).** 같은 줄에 왼쪽으로 정렬된 제목과 오른쪽으로 정렬된 부제입니다. 개발자 가이드는 다음 문서를 확인하세요.

<img width="274" alt="7" src="https://user-images.githubusercontent.com/40762111/76539025-8d491a00-64c3-11ea-8e97-7fe2c71713ee.png">

**Left Detail (Value 2).** A right-aligned title, followed by a left-aligned subtitle on the same line. For developer guidance, see [UITableViewCellStyleValue2](https://developer.apple.com/documentation/uikit/uitableviewcellstyle/uitableviewcellstylevalue2) constant of [UITableViewCell](https://developer.apple.com/documentation/uikit/uitableviewcell).

> **Left Detail (Value 2).**  오른쪽으로 정렬된 제목과 같은 줄 왼쪽으로 정렬된 부제입니다. 개발자 가이드는 다음 문서를 확인하세요.



All standard table cell styles also allow graphical elements, such as a checkmark or disclosure indicator. Of course, adding these elements decreases the space available for titles and subtitles.

> 모든 기본의 table cell 스타일은 또한 체크 표시나 disclosure과 같은 그래픽적인 요소를 사용할 수 있습니다. 물론, 이런 요소들을 추가하면 제목과 부제를 위한 공간이 줄어들게 됩니다.



**Keep text succinct to avoid clipping.** Truncated words and phrases are hard to scan and decipher. Text truncation is automatic in all table cell styles, but it can present more or less of a problem depending on which cell style you use and where truncation occurs.

> **자르는 것을 피하기 위해서 텍스트를 간결하게 유진하세요.** 잘린 단어나 구문들은 훑거나 읽어내기 어렵습니다. 텍스트를 자르는 것은 자동적으로 모든 table cell styles에 있지만, 어떤 cell 스타일은 사용하는지, 어디에서 잘리는는지에 따라서 큰 문제가 될 수도 되지 않을 수도 있습니다.



**Consider using a custom title for a Delete button.** If a row supports deletion and it helps provide clarity, replace the system-provided Delete title with a custom title.

> **삭제 버튼에 custom 제목을 사용하세요.** 행이 삭제 기능을 제공하고 간결하다면, 시스템에서 제공하는 삭제 제목을 custom 제목으로 대체하세요.



**Provide feedback when a selection is made.** People expect a row to highlight briefly when its content is tapped. Then, people expect a new view to appear or something to change, such as a checkmark appearing, that indicates a selection has been made.

> **선택이 만들어질 때, 피드백을 제공하세요.** 사용자는 행에 있는 콘텐츠가 탭 되었을 때, 간단하게 강조되는 것을 기대합니다. 그리고는 선택에 의해 나타나는 체크 표시가 등장과 같이 새로운 뷰가 나타나거나 무언가가 변경되기를 기대합니다.



**Design a custom table cell style for nonstandard table rows.** Standard styles are great for use in a variety of common scenarios, but some content or your overall app design may call for a heavily customized table appearance. To learn how to create your own cells, see [Customizing Cells](https://developer.apple.com/library/content/documentation/UserExperience/Conceptual/TableView_iPhone/TableViewCells/TableViewCells.html#//apple_ref/doc/uid/TP40007451-CH7-SW18) in [Table View Programming Guide for iOS](https://developer.apple.com/library/content/documentation/UserExperience/Conceptual/TableView_iPhone/AboutTableViewsiPhone/AboutTableViewsiPhone.html).

> **표준이 아닌 표의 행에서 custom table cell을 디자인하세요.** 표준의 스타일은 다양한 일반적인 상황에서 사용하기에 적합하지만, 어떤 콘텐츠 또는 전체적인 앱 디자인은 기본으로부터 꽤 변경된 표를 요구할 수도 있습니다. Custom된 cells 만드는 방법을 배우기 위해서 다음 문서를 확인하세요.



For developer guidance, see [UITableViewCell](https://developer.apple.com/documentation/uikit/uitableviewcell).

> 개발자 가이드는 다음 문서를 확인하세요.