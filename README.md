# 심박수 기반 영화 순위 제공 서비스

## 1. 아이디어 선정

![Untitled](https://user-images.githubusercontent.com/28921379/117543950-09a0a400-b05a-11eb-8a2a-b5054fa86afa.png)

사진 출처 : 코메디 닷컴 - 공포영화 '좋은 스트레스'로 작용 (연구)

공포영화 시청 시 검색을 통해 평가나 별점 순위 같은 지표를 보고 시청하면 재미가 없거나 기대치를 충족하지 못하는 경우가 빈번히 있습니다. 그 이유는 평가를 좋게 만들어주는 알바 등에 의해 가짜 평가가 많이 존재하기 때문입니다. 실제로 재미가 별로 없거나 혹은 너무 재미없는 영화들도 당장 검색해보면 평점이 엄청나게 낮다거나 평가가 안좋다거나 하는 부분은 거의 없고, 다 평균치 이상을 기록하는걸 볼 수 있습니다. 이에 좀 더 정확한 지표가 필요하다고 생각하였고 공포 영화 시청 할 때 증가하는 심박수를 분석하여 새로운 서비스를 만들어보려고 합니다.

재밌다고 말하는 공포영화는 보통 무서운 장면이 많이 나와서 공포를 많이 느낄 수 있는 영화인데, 이 영화의 심박수 증가량이 신빙성이 있는 지표인지를 알아보기 위해 조사를 진행했습니다.

조사한 자료에 따르면 첫번째로 공포영화를 봤을 때의 우리몸에서 일어나는 변화에 대한 자료인데, 공포영화를 보며 무섭다는 감정이 드는 이유는 뇌에서 공포를 관장하는 고신 편도체가 그 역할을 수행하는 것을 알 수 있었습니다. 무서운 장면을 본 이후에는 편도체에 자극이 전달되어 이곳의 활동이 급속도로 증가하기 시작하는데, 편도체가 활발해지면 우리몸은 위험에 대처할 준비를 하게 됩니다. 이에 따라 **심장박동수**와 호흡이 빨라지고 동공과 기도가 확장됩니다. 또한 혈압이 높아지고 근육이 경직되는 반응이 일어나기도 합니다. 그 결과 혈관이 이완하지 못해, 피가 충분히 돌지 않아 피부 온도가 낮아지고 서늘한 느낌이 들게 되는 것인데, 이처럼 편도체에 의한 자율신경계 반응으로 공포를 느끼게 됩니다. 또한 공포영화를 본 후, 몸에서는 아드레날린 등의 신경물질이 분비되어 짜릿한 체감과 더불어 카타르시스를 느끼게 되고 이는 공포영화를 통해 스트레스를 해소하고자 하는 이유이기도 합니다.

두번째로 실제 실험 사례가 있었습니다. 이전에 심박수를 이용해 순위를 매겨놓은 실험 결과들이 있었는데, 먼저 영국 런던에 본사를 둔 네트워크 회사 Broadband Choice 에서 평균 심박수 증가량을 기반으로 무서운 공포영화 순위를 실험했습니다. 실험은 공포 영화 50편을 50명의 성인 남녀가 시청하고 전후 평균 심박수를 비교하는 방식으로 진행했는데, 평균 심박수 상승률 상위권에 인시디어스, 살인소설, 컨저링 등 유명하고 재밌다고 평가가 된 영화들이 자리했고, 이를 보아 심박 수는 공포영화의 재미를 측정하는데 유의미한 데이터라고 판단할 수 있었습니다. 이 심박수를 분석하여 영화의 재미 정도를 나타내주는 서비스를 만들면 신빙성 있는 영화의 평가정보와 함께, 영화를 선택하는 새로운 지표를 제공해 줄 것이라고 생각합니다. 

</br>

## 2. 사례 분석

 - ### **심박수 모니터링을 통해 영화와 심박수 사이의 관계 이론 증명**
 *Apple Watch 또는 Fitbit과 같은 모니터링 기기가 항상 100 % 정확한 것은 아니므로 과학이 완벽하지 않습니다. 그러나 A24의 "심박수 도전"은 끔찍한 영화가 우리 몸에 실제적인 신체적 변화를 일으킬 수 있음을 분명히 상기시켜줍니다.*
 [https://mashable.com/2018/06/06/hereditary-heart-rate-challenge/](https://mashable.com/2018/06/06/hereditary-heart-rate-challenge/)

 - ### **HeartMonitor apple watch 앱**
 *개발자 Zach Simone은 시작할 수있는 "세션"내에서 심박수를 지속적으로 추적하고 운동 링에 포함되지 않는다는 간단한 목표를 염두에두고 HeartMonitor를 만들었습니다. "*
 *HeartMonitor는 회의 연설이나 프레젠테이션을 할 때, 축구 경기의 죽어가는 순간, 공포 영화를 보는 등 긴장된 상황에서 심박수를 모니터링하는 데 유용합니다.*

 - ### **byHeart 프로젝트, "이제 당신의 심장으로 영화를 평가하세요"**
 *인간의 감정을 가장 솔직하게 표현할 수 있는 수단인 '심장박동수'로 영화를 평가한다는 흥미로운 프로젝트가 내년에 선보일 예정이라고 합니다. 애플워치용 앱인 'byHeart'가 그 주인공인데요, 애플워치의 캐치프레이즈인 '심박 센서가 당신을 가슴 깊이 이해합니다'를 가장 잘 구현한 새로운 방식이 될 듯합니다.*
 [https://macnews.tistory.com/2649](https://macnews.tistory.com/2649)

 - ### "공포영화 보면서 심박수 측정을" 이색 시사회
 *시사회에 참여한 관객은 “인시디어스3 영화만큼이나 실시간으로 심박수를 확인하는 것도 흥미로웠다”며 “영화가 클라이맥스를 향해 갈 때, 심박수도 따라 상승하는 것을 실시간으로 확인하며 내 몸의 반응을 구체적으로 느낄 수 있었다”고 이색체험의 느낌을 전했다.*
 [https://www.asiae.co.kr/article/2015061212384495139](https://www.asiae.co.kr/article/2015061212384495139)

 **이 밖에도 많은 사례들이 존재 합니다. 지금까지 나온 서비스나 사례는 모두 단순히 심박수만을 측정해서 최대, 최소만을 다루고 있습니다. 최대, 최소 뿐만하니라 실시간으로 저장되는 심박수를 분석해서 사람마다 무서운정도가 다르다는 것까지 고려하여 보다 정확한 지표를 제공할 것입니다.**

</br>

## 3. 개요

서비스를 시작하면, 사용자의 기본 정보 혹은 분석을 위한 기본정보를 얻기위해서 로그인 과정을 수행하게 됩니다. 로그인을 하고 홈화면이 나오면, 곧 바로 분석되어 나온 영화의 순위들을 확인할 수 있습니다. 위에서 말한것과 같이, 심박수를 분석하여 순위를 매기게 되는데, 심박수 분석에는 스마트워치를 활용할 것입니다. 

측정을 위한 기본적인 플로우는 스마트워치에서 얻은 영화 러닝타임 동안의 심박수를 스마트폰으로 전송하고, 전송된 정보는 서버내의 분석 서비스로 넘어가게 됩니다. 분석을 마친후에는 영화 통계정보에 반영하고, 본인이 측정한 영화에 대한 기록도 확인할 수 있도록 합니다. 스마트워치 어플리케이션의 경우에는 Tizen OS 를 쓰는 기기를 사용할 것이고, HTML, CSS 등 웹 스택으로 앱을 구성할 수 있기 때문에 빠른 프로토타입을 개발 할 수 있습니다.

또한 영화 티켓에 영화 시작정보와 영화명 등의 정보를 담은 QR 코드를 넣어서 어플리케이션 내에서 한번 찍어서 등록해 놓으면 자동으로 해당시간에 측정을 시작하게 되어, 시간에 맞춰서 측정을 시작하도록 수동으로 조작 해야하는 불편함을 없애려고 합니다. 

그렇게 분석되어 나온 영화의 순위 외에 기본적으로 갖춰야할 영화의 제목, 줄거리, 예고편, 커뮤니티 등의 정보를 제공하는 서비스를 생각하고 있습니다. 

</br>

## 4. 기능 정의

 📱 **Application**

![Untitled 1](https://user-images.githubusercontent.com/28921379/117543971-28069f80-b05a-11eb-97ba-08753eba2cd4.png)

![Untitled 2](https://user-images.githubusercontent.com/28921379/117543974-2937cc80-b05a-11eb-8f8b-8ecb2196cae3.png)

![Untitled 3](https://user-images.githubusercontent.com/28921379/117543975-2937cc80-b05a-11eb-9867-d3918ddc5635.png)

![Untitled 4](https://user-images.githubusercontent.com/28921379/117543976-29d06300-b05a-11eb-921b-211b8774d61c.png)

![Untitled 5](https://user-images.githubusercontent.com/28921379/117543978-29d06300-b05a-11eb-84dc-4f0b9caf708e.png)

![Untitled 6](https://user-images.githubusercontent.com/28921379/117543979-2a68f980-b05a-11eb-8e8d-e9b64b831a75.png)

![Untitled 7](https://user-images.githubusercontent.com/28921379/117543980-2a68f980-b05a-11eb-9f9c-d63276d6c1b1.png)

</br>

🖥️ **Machine Learning**

DB에서 영화 상영 전 심박수 측정치와 영화 상영 중 심박수 측정 치를 불러와서 이상치 값을 아웃라이어 알고리즘을 통해 제거한다. 수정된 데이터를 이용해 영화 상영 전의 평균 심박수, 상영 중의 최고점과 최저점의 심박수 평균을 구한다. 상영 전과 상영 중의 심박수 평균치를 비교해 심박수 상승률을 계산하여 상승률이 높은 순서로 영화의 순위를 책정할 것이다.

</br>

- **아웃라이어 알고리즘**

    Boxplot(IQR) 방법

![Untitled 8](https://user-images.githubusercontent.com/28921379/117544023-52f0f380-b05a-11eb-82fa-1a8f3cb3e638.png)

사분위 값의 편차를 이용하는 방법으로, 사분위는 데이터를 값이 높은 순으로 정렬하고 1/4씩 쪼갠 것을 뜻한다. 그래서 25%, 50%, 75%, 100% 지점을 각 Q1, Q2, Q3, Q4로 정의하고, 분류 식을 정의하면 IQR = Q1~Q3 즉 IQR = Q3 - Q1 이 된다. 보통 사용하는 상수인 1.5를 곱해서 IQR * 1.5 + Q3 = 최대값(MAX OUTLIER), IQR * 1.5 - Q1 = 최소값으로 정의해서 최대값보다 높은 값과 최소값보다 낮은 값을 이상치로 판단해 제거하는 알고리즘입니다. 이렇게 정리된 데이터는 아래 그림과 같이 선형회귀 와 비슷한 분포를 가지게 됩니다.

![Untitled 9](https://user-images.githubusercontent.com/28921379/117544028-53898a00-b05a-11eb-8e75-59daa9510fca.png)

</br>

## 5. 설계

![Untitled 10](https://user-images.githubusercontent.com/28921379/117544029-54222080-b05a-11eb-8515-2d362484bbe2.png)

🍎**FrontEnd**

- Android Studio
- Tizen Studio

🍏**BackEnd**

- Spring Boot
- Flask
- MariaDB

🔳**DevOps**

- NCP(Naver Cloud Platform) - Effective Log Search & Analytics, Compute Sever
- Jenkins
- Docker
- Nginx
- Git / GitHub

</br>

클라이언트에서 작동되는 어플리케이션은 스마트폰의 경우 Android Studio, 스마트워치의 경우 Tizen Studio로 개발할 것이며, 스마트워치는 팀원이 가지고 있는 기기를 활용할 예정입니다.

클라우드 컴퓨팅 환경으로는 **Naver Cloud Platform**을 사용할 예정이며, 해당 클라우드 서비스에 있는 **Compute Server**를 사용하여 서버를 구축할 것이고, 제공되는 로그 분석 서비스인 **Effective Log Search & Analytics**를 사용할 예정입니다.

서버 내부에서는 컨테이너를 관리해줄 **Docker**와 CI/CD를 담당하는 **Jenkins**를 사용합니다. Jenkins의 경우에는 Naver Cloud Platform에서 무료 서비스로 제공해주는 것으로 확인되어 같이 연동해서 개발할 것이며, 컨테이너에는 영화 정보 제공, 사용자 관리, 데이터 분석, 결과를 서빙하는 기능을 위해서 Java 기반 **Spring Boot** 프로젝트와 Python 기반 **Flask,** 그리고 데이터베이스인 **MariaDB**가 배포될 예정입니다. html문서나, CSS 처리는 하지 않고, REST API를 주로 사용할 예정이기 때문에, Apache보다 단순하고 동시접속 처리에 특화된 **Nginx**를 사용하여 웹서버를 구축할 것입니다.

형상관리와 더불어 CI/CD에 WebHook을 제공하는 **Git**을 사용합니다. 그리고 **GitHub**를 통해서 개발중에 발생하는 이슈와 문제점들을 팀원이 공유하고, 같이 해결할 것입니다.

⭐ **고려사항**

개발하려는 서비스의 인프라의 경우 Naver Cloud Platform에서 제공되는 로그 분석과 Jenkins 등을 활용하여 진행할 예정이지만, CI/CD와 로그분석 등 다양한 기능을 통합 제공하는 **ACCORDION**을 활용하여 좀 더 효율적으로 서비스가 동작하는 방향으로 개발 초기에 방향을 잡을 예정입니다.

</br>

## 6. 기대효과

- 스마트워치 와 비슷한 장비를 이용했지만, 심박수 측정만 가능하다면, 어떠한 장비 어느 장소에서든 사용할 수 있다.
- 심박수라는 조작이나 은닉이 불가능한 데이터를 이용하여 평가에 신뢰성을 높일 수 있다.
- SNS를 통해 심박수 체크등 신선한 아이템을 제공함으로써, 영화의 흥행을 기대해볼 수 있다.
- 작품성이 좋지만, 리뷰가 별로 없어 흥행하지 못하고 묻히는 영화들을 발굴할 수 있다.

</br>

## 7. 팀원 소개

### **김도현 (팀장)**

- ML Engineer
- 분석 서비스 개발
- 결과 서빙 API 구현

### 박윤정 **(팀원)**

- ML Engineer
- 분석 서비스 개발
- 결과 서빙 API 구현

### **김가람 (팀원)**

- Backend Engineer
- 서버 관리
- 인프라 구축
- REST API 구현

### 윤혜수 **(팀원)**

- Frontend Engineer
- 클라이언트 개발
- UX/UI 구성
- 하드웨어 통신 구현
