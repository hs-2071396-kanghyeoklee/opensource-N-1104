# OSRM 

- C++로 작성된 고성능 라우팅 엔진으로, OpenStreetMap 데이터에서 실행되도록 설계되었다.

- OSRM은 무료 네트워크 서비스이며, Linux, FreeBSDm Windows 및 Mac OS X 플랫폼을 지원한다.

- OSRM은 오픈소스이므로 범위 내에서 원하는 로직으로 customization이 가능하다.

- 네이버나 구글지도 API와 달리 OpenStreetMap과 OSRM을 활용하면 비용이 들지 않는다는 장점이 있다.

- HTTP API, C++ 라이브러리 인터페이스, NodeJs wrapper를 통해 사용할 수 있는 OSRM 서비스는 다음과 같다.

  - **Nearest** - 거리 네트워크에 좌표를 스냅하고 가장 가까운 일치 항목을 반환

  - **Route** - 좌표 사이에서 가장 빠른 경로를 탐색

  - **Table** - 제공된 모든 좌표 쌍 사이의 가장 빠른 경로의 지속 시간 또는 거리 계산

  - **Match** - 가장 타당한 방법으로 노이즈가 많은 GPS 추적을 도로 네트워크에 스냅

  - **Trip** - 탐욕 알고리즘을 사용하여 TSP(Travelling Salesman Problem)을 해결

    *탐욕 알고리즘 : 각 단계에서 국소적으로 최적의 선택을 하는 문제 해결 휴리스틱을 따르는 알고리즘이다.

    *TSP : 일련의 지점과 방문해야 하는 위치 사이의 최단 경로를 찾는 임무를 맡은 알고리즘 문제

  - **Tile** - 내부 라우팅 메타데이터가 있는 맵박스 벡터 타일 생성

    *맵박스 : 맞춤형 디자인 맵을 위한 오픈소스 매핑 플랫폼

    *벡터 타일 : 점, 선 및 다각형과 같은 지리공간 벡터 데이터를 저장하기 위한 경량 데이터 형식

    

    

    ![image](https://user-images.githubusercontent.com/109498876/204121960-a500bca6-8b4e-4bbd-9f84-75d45caa44dd.png)OSRM demo page 동작 화면



- Related [Project-OSRM](https://github.com/Project-OSRM) repositories:

  - [osrm-frontend](https://github.com/Project-OSRM/osrm-frontend)  

    User-facing frontend with map. The demo server runs this on top of the backend

  - [osrm-text-instructions](https://github.com/Project-OSRM/osrm-text-instructions)  

    Text instructions from OSRM route response

  - [osrm-backend-docker](https://hub.docker.com/r/osrm/osrm-backend/)  

    Ready to use Docker images



### OpenStreetMap 개념 및 라이선스

OpenStreetMap은 누구나 참여할 수 있는 오픈소스 방식의 무료 지도 서비스입니다. 

ODbL 라이선스가 적용되는 오픈스트리트맵으로 이미지 파일 등을 만들었을 때는, 저작자((c)OpenStreetMap Comtributor) 표기만 한다면 어떤 라이선스로든 배포가 가능합니다. 단, 오픈스트리트맵을 활용해 새로운 '데이터베이스'를 만들었거나, 오픈스트리트맵 데이터베이이스를 그대로 활용하지 않고 데이터베이스를 수정한 뒤 수정한 DB로 작업물을 만들었을 경우, 해당 데이터베이스를 ODbL 라이선스로 배포해야 합니다.







# OSRM license

- **OSRM은 “simplified BSD 라이선스”라고 알려진 BSD-2-Clause 버전 라이선스**

 

조건이 충족될 경우 수정 여부에 관계없이 소스 및 이진 형식의 재배포 및 사용이 허용됩니다.



소스 코드의 재배포는 위의 저작권 고지, 이 조건 목록 및 다음 고지 사항을 유지해야 합니다.
 바이너리 형식의 재배포는 위의 저작권 고지, 이 조건 목록 및 배포와 함께 제공된 문서 및 기타 자료에 다음 고지 사항을 복제해야 합니다.

 

본 소프트웨어는 저작권 소유자 및 기여자에 의해 "있는 그대로" 제공되며, 상품성 및 특정 목적에 대한 적합성에 대한 묵시적 보증을 포함하지만 이에 국한되지 않는 명시적 또는 묵시적어도 이에 국한되지 않습니다. 그러나 어떠한 경우에도 저작권 소유자 또는 기여자는 계약상 책임이 있는지 여부에 관계없이 어떠한 직접적, 간접적, 부수적, 특별한, 모범적 또는 결과적 손해(대체 상품 또는 서비스의 조달, 사용, 데이터 또는 이익의 손실, 또는 업무 중단을 포함하지만 이에 국한되지 않음)에 대해서도 책임을 지지 않습니다. 그러나 본 소프트웨어의 사용에서 발생하는 계약상, 엄격한 책임 또는 불법행위(과실 또는 기타 포함)에 관계없이 그러한 손상의 가능성에 대해 고지된 경우에도 모든 책임 이론을 야기합니다.







# Docker

- 도커 컨테이너 기술은 2013년 오픈소스 도커 엔진으로 출시되었다.

- Docker는 워크플로우를 단순화하고 가속화하는 동시에 개발자가 각 프로젝트에 대해 툴, 애플리케이션 스택 및 구축 환경을 선택하여 자유롭게 혁신할 수 있도록 지원하는 오픈소스 프로젝트이다.

![image](https://user-images.githubusercontent.com/109498876/204122061-3ef51d38-9531-4ca4-95af-9b11d01a8550.png)Docker로 애플리케이션 컨테이너화



- Docker는 아래의 기능들로 애플리케이션의 복잡성을 극복할 수 있다.
  - **Keep It Simple** - 친숙한 CLI 기반 워크플로우는 모든 기술 수준의 개발자가 컨테이너형 응용프로그램을 구축, 공유 및 실행
  - **Move Fast** – 단일 패키지에서 설치하여 몇 분 만에 실행 가능. 개발과 생산 간의 일관성을 보장하면서 로컬에서 코드를 작성하고 테스트함
  - **Collaborate** – 커뮤니티에서 제공되는 인증된 이미지를 프로젝트에 사용 가능. 클라우드 기반 응용프로그램 레지스트리에 푸시하고 팀 구성원과 협업







# Docker license

- **Apache License 2.0**



귀하가 본 문서의 조건을 준수한다는 조건으로 Docker는 해당 구독 기간 동안 귀하가 선택한 제품에 설명된 대로 서비스를 다운로드, 설치 및 사용할 수 있는 제한적이고 비독점적이며 양도 불가능하고 서브라이선스를 부여할 수 없는 라이선스를 귀하에게 부여합니다. 서비스의 일부가 오픈 소스 소프트웨어를 포함하거나 활용하는 경우 해당 오픈 소스 소프트웨어는 해당 배포 또는 해당 도움말, 고지 사항 또는 소스 파일에 참조된 오픈 소스 라이선스 계약의 조건에 따라 배포되거나 제공됩니다. 오픈 소스 소프트웨어에 대한 저작권 및 기타 소유권은 해당 배포 또는 해당 도움말, 공지, 정보 또는 소스 파일에서 식별된 저작권 소유자가 보유합니다.



### Docker 이미지를 이용한 OSRM backend 구축

1. Geofabrik에서 한국 지도 파일 다운로드

2. Docker 이미지 생성 및 지도 파일 전처리

   *Docker 이미지 : 특정 프로세스를 실행하기 위한(컨테이너 생성에 필요한) 모든 파일과 환경을 지닌 파일

3. Docker 서버 실행







# DFD 서식

![image-20221125153950397](https://user-images.githubusercontent.com/109498876/204122110-ff6d9965-540a-4e59-acf6-6092207a6b1b.png)







출처

https://github.com/Project-OSRM

https://www.docker.com

https://github.com/confluentinc/common-docker/blob/master/LICENSE-Apache

https://forum.openstreetmap.org/viewtopic.php?id=72292