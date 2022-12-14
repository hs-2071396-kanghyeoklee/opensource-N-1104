# Saleor

---

* python 및 Django를 기반으로 서비스를 제공 하는 전자 상거래(E-commerce) 오픈소스이다.

* github에서도 별점이 19,000개가 넘는 상당히 인기 있는 프로젝트이다.

* 배달과 매장이 연동되어 결제 단계를 구축할 때 사용하게 되는 오픈소스이다.

  

### 서비스의 필요 이유 및 상세 분석

#### 라이선스 무료

* 오픈소스로 공개된 saleor는 무료로 사용이 가능한 점이 가장 큰 장점이다.

* Open Software License 버전 3.0(OSL-3.0)으로 게시된다.

  

#### 간편한 설치

* 개발 환경이 Docker로 설정되어 있기에 개발 환경을 따로 설치할 필요가 없다.

* 오픈소스를 다운로드 후 실행이 몇 개의 커맨드 실행으로 가능하다.

  
  
  

###### 1. 프로젝트 다운로드, 도커 빌드

```

git clone https://github.com/saleor/saleor-platform.git --recursive --jobs 3

cd saleor-platform

docker-compose build

```

###### 2. 프로젝트에 필요한 테이블 생성

```

docker-compose run --rm api python3 manage.py migrate

docker-compose run --rm api python3 manage.py collectstatic --noinput

```

###### 3. 샘플 데이터 생성

```

docker-compose run --rm api python3 manage.py populatedb

```

###### 4. 서버 실행

```

docker-compose up

```

  

#### 잘 정리된 도큐먼트

* 기능별 매뉴얼이 잘 정리되어 있다.

* 검색도 가능하며 문서를 한글로 변역하면 충분히 볼 수 있을 정도로 잘 정리되어 있다.

#### 디자인 UI/UX

* 기존의 이커머스 사이트들은 기능면을 중요시하다 보니 전체적인 디자인과 UI/UX의 퀄리티가 좋지 않은 경우가 많다.

* saleor만의 독특한 콘셉트와 디자인 UI/UX는 상당히 퀄리티가 높다는 걸 알 수 있다.

  

#### 버그 대응 유지 보수

* saleor의 최신 버전은 3.8.0이며 최근인 10/28일에도 업데이트가 되었다.

* 이 글을 작성하는 2022/11월을 기준으로 불과 며칠 전에 업데이트가 이뤄졌다.

* 업데이트가 활발히 이뤄지는 프로젝트라는 걸 알 수 있다.

  

#### 사이트 통계와 제품 관리를 위한 대시보드

* 대시보드는 사용자와 관리자의 주문, 상품 등록 수정, 삭제, 결제, 통계 등의 기능을 볼 수 있게 여 꼭 필요한 기능이다.

* 가독성도 좋아야 하며 다양한 기능이 지원되어야만 한다.

* saleor의 대시보드 역시 사용자 친화적이며 등 EC 사이트 운영에 필요한 다양한 기능을 갖췄다.

  

#### 모바일 버전

* 최근 이커머스 사이트는 모바일의 접속이 더 많다.

* saleor의 경우 모바일 접속 시 모바일 버전을 지원하고 있다.

  

#### saleor 특징

1. GraphQL API : 단일 요청 등으로 많은 리소스 가져 오기 가능

2. 다채널 : 가격, 통화, 주식, 제품 등의 채널별 제어가 가능

3. CMS : 다양한 제품의 카탈로그를 관리할 수 있는 기능

4. 대시보드 : 사용자 친화적이고 빠르며 생산적이며 관리 용이

5. 글로벌 디자인 , 다중 언어, 다중 창고 지원

6. 주문 : 주문, 발송, 환불을 위한 종합시스템 지원 

7. 장바구니 : 할인 및 프로모션을 완벽하게 제어하는 선지급 및 세금 옵션

8. 결제 : 유연한 API 아키텍처로 모든 결제 수단 통합 가능

9. SEO : 더 많은 고객에게 제품이 노출되는 최적화된 SEO

10. 간편한 클라우드 배포 : Docker를 사용한 배포에 최적화

  

## 활용 계획

  

* 사용자의 기호에 맞춰 추천해준 메뉴와 그에 맞는 매장을 매칭해준 서비스에서 결제 단계로 넘갔을 때 Saleor가 사용된다.

* Django 로 백앤드 서버를 구성한다. Python 으로 작성되며 , SQLite 데이터베이스에서 상태를 유지-관리한다. 그런 다음 제품의 카탈로그, 주문, 장바구니 결제 등을 인터페이스로 구현하는 Saleor Dashboard를 구성하고 관리하게 된다.
