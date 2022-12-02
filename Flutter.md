1.Flutter란?

Flutter는 Google에서 개발하고 Mobile World Congress 2018에서 최초 베타 릴리스를 발표하면서 새롭게 소개된 크로스 플랫폼 모바일 앱 개발 프레임워크입니다.
또한 개발자가 iOS와 Android 두 OS에 대해 고품질 기본 인터페이스를 제작하는 데 도움을 주는 크로스 플랫폼 프레임워크라고 할 수 있습니다.
기존 UI를 모두 버리고 자체적으로 UI를 렌더링하기 때문에 iOS에서 material 디자인과 ripple 애니메이션 을 볼 수 있고 Android 에서 cupertino 디자인을 볼 수 있습니다.
마치 화면 전체를 2D 그래픽 API로 fillRect 하고 drawText drawImage 해서 앱을 만드는 것처럼 Flutter 엔진이 Skia 기반으로 렌더링 해줍니다. 웹 개발에서 HTML을 모두 무시하고 전체를 flash나 canvas로 만드는 것과 같습니다.

2.왜 CrossPlatform을 사용할까요?

모바일 개발의 경우 iOS와 Android 모바일 개발자가 각각 따로 있다면 꼭 크로스 플랫폼으로 앱을 개발하지 않아도 됩니다. 하지만, 각 OS 별로 유저들에게 동일한 UI와 UX를 제공하면서 개발한다는 것은 쉬운일도 아닐뿐더러 각각 전문 개발자들이 필요하게 되니 개발 자원이 2배이상 필요하게 됩니다. 그리고 한 명의 개발자가 둘다 개발을 한다고 가정하면 각 OS의 개발 방식이 서로 다르기 때문에(IDE, 개발언어, 툴 등등) 따로 공부해야하는 필요성도 있습니다.

설령 개발을 완료 했다 하더라도 앱의 유지보수가 쉽지 않다는 단점이 있습니다. 안드로이드, IOS 따로 유지보수(추가 기능, 오류, 앱스토어 관리 등등) 관리를 해야하기 때문입니다.
그래서 크로스 플랫폼을 사용한다면 우선 개발 자원을 줄일 수가 있습니다. 하나의 프레임워크로 안드로이드, iOS 모두를 동시 개발이 가능하기 때문입니다.
관리 역시도 하나의 개발 소스만 관리하면 해결되기 때문에 훨씬 편리합니다.

하지만 이미 시장에는 모바일 크로스플랫폼 개발하면 떠오르는 프레임워크로 Facebook에서 개발을 주도하는 React-Native가 있으며 많은 개발자분들이 React-Native와 Flutter를 두고 고민을 하는 상황입니다.

3. Flutter는 어떤 프로그래밍 언어를 사용하나요?

Flutter는 Google이 개발한 오픈 소스 프로그래밍 언어인 Dart를 사용합니다. Dart는 UI를 구축하는 데 최적화되어 있으며, Dart의 많은 강점은 Flutter에서 활용됩니다.
예를 들어 Flutter에서 사용되는 Dart의 기능 중 하나로 Sound Null Safety 기능이 있습니다. Dart의 Sound Null Safety는 null 오류라는 일반적인 버그를 손쉽게 감지할 수 있도록 해줍니다. 이 기능은 개발자가 코드 유지 관리에 허비하는 시간을 줄이고 애플리케이션 구축에 집중할 수 있는 시간을 더 확보해 줍니다.


4.Flutter의 위젯이란 무엇인가요?

Flutter에서 개발자는 위젯을 사용하여 UI 레이아웃을 만듭니다. 즉, 창과 패널부터 버튼과 텍스트에 이르기까지, 사용자가 화면에서 보는 모든 요소가 위젯으로 만들어집니다.
Flutter 위젯은 개발자가 손쉽게 사용자 지정할 수 있도록 설계되었습니다. Flutter는 구성 접근 방식을 통해 이를 실현합니다. 즉, 대부분의 위젯은 작은 위젯으로 구성되며, 가장 기본적인 위젯은 특정한 용도가 있습니다. 따라서 개발자가 위젯을 결합하거나 편집하여 새 위젯을 만들 수 있습니다.
Flutter는 플랫폼의 기본 제공 위젯을 사용하는 것이 아니라, 자체 그래픽 엔진을 사용하여 위젯을 렌더링합니다. 덕분에 사용자는 플랫폼 전체에 걸쳐 Flutter 애플리케이션에서 유사한 모양과 느낌을 경험할 수 있습니다. 또한 일부 Flutter 위젯은 플랫폼별 위젯에서는 수행할 수 없는 기능을 수행할 수 있으므로, 이러한 접근 방식은 개발자에게 유연성을 제공합니다.
Flutter는 커뮤니티에서 개발한 위젯도 손쉽게 사용할 수 있도록 합니다. Flutter의 아키텍처는 여러 위젯 라이브러리를 적용하는 기능을 지원하며, Flutter는 커뮤니티에서 새로운 위젯 라이브러리를 구축하고 유지 관리하도록 장려합니다.
Flutter 위젯의 유형
Flutter는 다운로드 할 때부터 광범위한 위젯 카탈로그와 함께 제공됩니다. 카탈로그에는 스타일링, Cupertino(iOS 스타일 위젯) 및 Material Components(Google의 재료 설계 지침을 따르는 위젯)를 비롯한 14개의 범주가 있습니다.
Flutter에는 레이아웃과 테마도 포함되어 있어 개발자가 빠르게 구축하는 데 도움이 됩니다.

5.Flutter는 어떻게 지원되나요?
Flutter는 Google과 Reddit, Discord, Slack, Stack Overflow, Gitter의 활성 오픈 소스 커뮤니티에서 지원합니다. Google은 2018년 출시 이후 꾸준히 Flutter를 업데이트해 왔으며, 여기에는 macOS와 Linux로 안정적 지원을 확장한 2022년 Flutter 3 업데이트가 포함됩니다.
Flutter를 쉽게 익힐 수 있도록 Google은 Flutter 사이트에서 광범위한 문서와 자습서를 제공합니다. Flutter 사용자와 소통하기 위해 Google은 글로벌 이벤트를 열고 커뮤니티 프로젝트를 홍보하며 개발자의 도전을 후원하고 있습니다. 예정된 이벤트는 Flutter 사이트에서 확인할 수 있습니다.
Flutter 커뮤니티에서는 개발자 경험을 간소화하는 수천 가지 서드 파티 패키지와 뛰어난 도구를 만들어냈습니다. 이러한 라이브러리는 pub.dev에서 사용할 수 있습니다.

6.Flutter 라이센스 
 
BSD 라이센스로 소스코드 공개의 의무가 없으며 상용(상업적) 소프트웨어에서도 무제한 사용이 가능한 라이센스로 저작권자 표기, 보증 부인만 준수하면 소스코드의 변경 & 배포에 아무런 제한을 받지 않습니다.

​​​

장점

통합 개발 환경 지원
Flutter는 다양한 Editor(Android Studio, VS Code 등등)를 사용하여 빌드가 가능합니다.
Android Studio는 Flutter Inspector와 Flutter Outline이라는 개발 도구를 추가적으로 지원해줍니다. VS code 에서는 간단하게 Extension 으로 Flutter를 설치하여 Flutter를 사용할 수 있습니다.

성능 문제 해결
기존 React Native 혹은 Hybrid App의 경우 네이티브 브릿지를 통한 통신이 불가피했습니다. 하지만 Flutter는 직접 컴파일되서 Render를 직접 하기때문에 성능이 빠릅니다. 애니메이션 속도가 60프레임은 가뿐히 넘어서는 것이 기존 크로스 플랫폼시장의 주류였던 React Native와 Flutter를 비교하는 많은 글들에서 Flutter를 내세우는 부분입니다.

머티리얼 디자인과 쿠퍼티노
Flutter는 Androd와 iOS의 대표 디자인 가이드를 기본적으로 제공합니다.
구글의 머티리얼 디자인(Material Design)의 홈페이지에는 이미 Flutter가 포함되어 있고 가이드만 제공하는 것 뿐만아니라 Flutter 프로젝트에 바로 추가하여 사용할 수 있는 패키지도 제공합니다.
안드로이드와 iOS에서 같은 머티리얼 디자인을 사용하더라도 플랫폼에 따라 다르게 출력되는 부분을 각각 디자인 가이드에 맞게 화면을 그립니다.
iOS앱을 개발하는 경우 iOS특유의 디자인 시스템인 쿠퍼티노(Cupertino) 위젯을 제공합니다.
그렇기에 선택의 폭이 정해져 있기 때문에 어떤 UI 라이브러리를 사용할 것인지 고민 할 필요가 없습니다만 이건 장점이자 단점이 될수도 있습니다.

Dart를 사용하지만 Native 코드도 사용
앞서 Dart를 사용한다고 했지만 결국엔 크로스 플랫폼이기에 해당 OS에 최적화된 앱을 만들려면 Native 코드를 사용할수밖에 없고 Dart와 섞어서 사용을 합니다.
즉, Dart만 사용하는것이 아니라 Android면 Kotlin, iOS면 Swift도 사용합니다.
이는 기존의 Native 코드를 사용한 개발자라면 장점이 됩니다.


단점
Flutter의 경우 Github 이슈란에 가보면 엄청난 이슈가 올라와 있는 것이 눈에 보입니다.
물론 이는 Flutter 자체가 이슈 항목에 아무나 이슈제의가 가능하도록 했기 때문에 그런점도 있습니다.

여기서 몇가지만 정리 하도록 하겠습니다.

Native API를 Dart에서 직접 호출 불가합니다.
특별히 심하게 문제가 되진 않지만 외부 플러그인을 써야합니다.

Code Pushing
코드를 고치려면 새 버전을 배포해야 합니다.
React Native, Cordova, Ionic 에선 이미 지원 중 입니다.
https://github.com/flutter/flutter/issues/14330

Air BNB Lotti 사용 불가합니다.
Flutter는 지원하지 않습니다.
Android, iOS, React-Native만 지원
로티는 어플리케이션에 Fancy 한 에니메이션을 넣어주는 라이브러리이며 제가 개인적으로 좋아하는 라이브러리 입니다.
https://airbnb.design/lottie/

웨어러블 디바이스앱에 약합니다.
https://pub.dev/packages/wear
위 플러그인이 있지만 Native 마냥 쉽게 되지 않습니다.

C/C++ 라이브러리 호출이 안됩니다.
NDK C/C++ 라이브러리 호출이 Dart에서 안됩니다.
외부 플러그인을 써야하고, 원하는 플러그인이 없다면 만들어야 하는데 이는 보통일이 아닙니다.

지원되는 플러그인이 부족하다.
아직 플러그인들은 부족한 편입니다.
어플을 생성할 때, Webview, Map 등 플러그인은 필요합니다.
하지만 Flutter의 이러한 플러그인들은 전부 0.4, 0.3 등등 1.0을 넘는 버전을 보기가 힘듭니다. 따라서 지속적으로 업데이트가 되고있고, 업데이트가 될때마다 다시 붙이고 테스트해보는 것은 어마어마하게 번거로운 일이 될 것입니다.

아직까진 국내에 개발관련 자료가 많이 없다.
Android, iOS Native는 나온지 오래되서 자료가 많다보니 문제해결이 쉽습니다만, 국내엔 아직까진 자료가 많다고 할수가 없어 이슈 상황 발생시 자료 찾기가 어렵습니다.
또한, Flutter 개발자들도 그렇게 많은 편이 아니기에 도움을 구하기도 어느정도 힘이 듭니다.


참고내용
https://flutter-ko.dev/docs
https://jaceshim.github.io/2019/01/22/flutter-study-about-flutter/index.html
https://engineering.linecorp.com/ko/blog/flutter-pros-and-cons/
https://sambalim.tistory.com/33
https://aws.amazon.com/ko/what-is/flutter/
