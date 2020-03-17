# Image Size and Resolution
The coordinate system iOS uses to place content onscreen is based on measurements in points, which map to pixels in the display. A standard-resolution display has a 1:1 pixel density (or @1x), where one pixel is equal to one point. High-resolution displays have a higher pixel density, offering a scale factor of 2.0 or 3.0 (referred to as @2x and @3x). As a result, high-resolution displays demand images with more pixels.

> iOS가 콘텐츠를 화면에 배치하기 위해 사용하는 좌표 시스템은 디스플레이의 픽셀에 매칭되는 포인트의 측정에 기초합니다. 표준 해상도 디스플레이는 1:1 화소 밀도(또는 @1x)를 갖고 있는데, 하나의 픽셀은 하나의 포인트와 같습니다. 고해상도 디스플레이는 2.0 또는 3.0(@2x와 @3x라고 하는)의 배율을 제공하여 더 높은 화소 밀도를 가지고 있습니다. 그 결과, 고해상도 디스플레이는 이미지에 더 많은 픽셀을 요구합니다.

<img width="552" alt="스크린샷 2020-03-17 오전 2 05 30" src="https://user-images.githubusercontent.com/40762111/76782826-365d8080-67f4-11ea-8b4c-18eba383238a.png">

For example, suppose you have a standard resolution (@1x) image that's 100px × 100px. The @2x version of this image would be 200px × 200px, and the @3x version would be 300px × 300px.

> 예를 들어, 100px * 100px의 표준 해상도 (@1x) 이미지를 가지고 있다고 가정해보세요. 이미지의 @2x 버전은 200px * 200px, @3x 버전은 300px * 300px이 됩니다.



**Supply high-resolution images for all artwork in your app, for all devices your app supports.** Depending on the device, you accomplish this by multiplying the number of pixels in each image by a specific scale factor.

> **앱이 지원하는 모든 기기를 위해서 앱 내의 모든 삽화에 대하여 고해상도 이미지를 제공하세요.** 기기에 따라서, 각각의 이미지의 픽셀 수를 특정 배율에 곱하여 이 작업을 수행합니다.



| Device           | Scale Factor |
| :--------------- | :----------- |
| 12.9" iPad Pro   | @2x          |
| 11" iPad Pro     | @2x          |
| 10.5" iPad Pro   | @2x          |
| 9.7" iPad        | @2x          |
| 7.9" iPad mini 4 | @2x          |
| iPhone XS Max    | @3x          |
| iPhone XS        | @3x          |
| iPhone XR        | @2x          |
| iPhone X         | @3x          |
| iPhone 8 Plus    | @3x          |
| iPhone 8         | @2x          |
| iPhone 7 Plus    | @3x          |
| iPhone 7         | @2x          |
| iPhone 6s Plus   | @3x          |
| iPhone 6s        | @2x          |
| iPhone SE        | @2x          |



### Designing High-Resolution Artwork

**Use an 8px-by-8px grid.** A grid keeps lines sharp and ensures that content is as crisp as possible at all sizes, requiring less retouching and sharpening. Snap the image boundaries to the grid to minimize half pixels and blurry details that can occur when scaling down.

> **가로 세로 8px 8px 그리드를 사용하세요.** 그리드는 선을 선명하게 유지하고, 모든 크기의 콘텐츠가 가능한 한 선명하게 유지되도록 하며 리터칭과 샤프닝(선명하게 하는 작업)을 덜 필요로 합니다. 이미지 경계를 그리드에 맞추어 스냅하고, 크기를 줄일 때 발생할 수 있는 반 픽셀들과 흐릿한 정보들을 최소화하세요.



**Produce artwork in the appropriate format.** In general, use de-interlaced PNG files for bitmap/raster artwork. PNG supports transparency and, because it's lossless, compression artifacts don't blur important details or alter colors. It's a good choice for intricate artwork that requires effects like shading, textures, and highlights. Use JPEG for photos. Its compression algorithm usually produces smaller sizes than lossless formats and artifacts are harder to discern in photos. Photo-realistic app icons, however, look best as PNGs. Use PDF for glyphs and other flat, vector artwork that requires high-resolution scaling.

> **적절한 형식의 삽화를 만드세요.** 일반적으로, 비트맵/래스터 작업을 위해서 여러 가지가 합쳐지지 않은 PNG 파일을 사용하세요. PNG는 투명도를 제공하고, 무손실이므로 압축 작품들이 중요한 디테일한 부분을 흐리지 않으며 색을 바꾸지 않습니다. 그림자, 질감, 강조와 같이 효과를 요구하는 복잡한 작품에 좋은 선택입니다. 사진은 JPEG를 사용하세요. JPEG의 압축 알고리즘은 보통 무손실 형식보다 더 작은 크기를 만들고, 사진에서 인위적인 부분을 알아차리기 더 어렵습니다.



**Use the 8-bit color palette for PNG graphics that don’t require full 24-bit color.** Using an 8-bit color palette reduces file size without reducing image quality. This palette is not appropriate for photos.

> **전체 24비트 색상이 필요하지 않은 PNG 그래픽에 8비트 색상 팔레트를 사용하세요.** 8비트 색상 팔레트를 사용하는 것은 이미지의 퀄리티를 유지하면서 파일 크기를 줄입니다. 이러한 팔레트는 사진에는 적합하지 않습니다.



**Optimize JPEG files to find a balance between size and quality.** Most JPEG files can be compressed without noticeable degradation of the resulting image. Even a small amount of compression can save significant disk space. Experiment with compression settings on each image to find the optimal value that yields an acceptable result.

> **사이즈와 퀄리티 사이의 균형을 찾기 위해서 JPEFG 파일을 최적화하세요.** 대부분의 JPEG 파일은 결과 이미지의 현저한 저하 없이 압축될 수 있습니다. 작은 압축이라고 할지라도 상당한 디스크 공간을 절약할 수 있습니다. 각 이미지의 압축 설정을 실험하여, 허용할 만한 결과 값을 도출하기 위한 최적의 값을 찾으세요.



**Provide alternative text labels for images and icons.** Alternative text labels aren’t visible onscreen, but they let VoiceOver audibly describe what's onscreen, making navigation easier for people with visual impairments.

> **이미지와 아이콘으로 대체 텍스트 labels를 제공하세요.** 대체 텍스트 labels는 화면 속에 표시되지는 않지만, 보이스오버가 화면 속의 내용을 청각적으로 설명할 수 있도록 도와주어, 시각 장애가 있는 사용자들이 쉽게 탐색할 수 있도록 합니다.