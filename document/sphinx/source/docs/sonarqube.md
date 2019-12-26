# 품질속성 지표 판독 및 목표 설정

### SonarQube가 제공하는 지표는 아래와 같다

#### Duplicate code 중복코드

> 한 클래스의 서로 다른 두 메소드 안에 같은 코드가 있거나, 동일한 수퍼클래스를 갖는 두 서브 클래스에서 같은 코드가 나타나는 경우임.
수정 사항이 발생했을때 같은 부분을 모두 수정해 줘야 하기 때문에 오류발생요인이 되기도 하며, 유지보수를 어렵게 하는 이유가 되기도 하기때문에 반드시 제거해야 한다.
>
> 목표 : 0 % 이상의 수치가 나오면 관리대상으로 분류하고 , "전체 소스 코드 중 코드 중복이 심한 영역(전체 중복 코드 비율, 우선 순위별 비율)을 식별해 중복 라인 수가 많은 코드부터 리팩토링(코드를 일반화, 재사용, 추상화)하며, 우선 순위가 High로 식별된 중복 코드는 모두 제거하고 우선순위가 Normal이나 Low로 식별된 중복 코드는 자율적으로 제거한다."
[출처] [독후감상] NHN
은 이렇게 한다! 소프트웨어 품질관리|작성자 취중선

#### Code coverage

> 테스트 코드 작성에 대한 개념 및 필요성을 초기에 전파.
>
> 테스트 자동화 프레임워크 도입을 검토
>
> 목표 : 60%/line , branch

#### Complex code 복잡도

> [기본개념] (http://story.wisedog.net/sw-metric-cyclomatic-complexity-%EB%B3%B5%EC%9E%A1%EC%84%B1-%EC%A7%80%ED%91%9C/)
>
> 목표 : 6 / function 이상인 것들을 리팩토링 대상으로 선정

#### Potential bugs

> Critial 은  10 이하, Major : 항목중 중요도가 상인 항목에 대해 리팩토링 대상으로 선정

#### Documentation

> 목표 : 70% 이상, undocument가 5 이상인 코드는 보완 대상으로 선정

#### Comment

> 30%이하의 코멘트 작성 소스에 대해 보완 대상으로 선정


## 참조
* [소프트웨어 아키텍처] (http://blog.naver.com/PostView.nhn?blogId=egmation&logNo=70175040398)
* [NHN은 이렇게 한다! 소프트웨어 품질관리] (http://blog.naver.com/PostView.nhn?blogId=lugenzhe&logNo=90102390361)