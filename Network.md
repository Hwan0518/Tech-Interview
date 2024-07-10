<details>
  <summary><h3> Restful API에 대해서 설명해주세요 <h3></summary>
    
- Restful API란 클라이언트와 서버간의 웹 통신을 위한 API중 하나로, REST 아키텍처 스타일을 따르는 API를 의미합니다.
- Restful API는 HTTP 메서드로 행위를 나타내고 URI로 자원을 명시하여 어떤 동작을 하는것인지 알아보기 쉬운 구조로 작성됩니다.
- 이는 Rest 성숙도 모델에 따라 총 4단계로 구분지을 수 있습니다.
    - 0단계는 단순히 HTTP 프로토콜을 사용하는 단계, 1단계는 개별 자원에 맞는 엔드포인트(end point)를 설정하는 단계, 2단계는 CRUD 행위에 따라서 적절한 HTTP Method를 사용하는 단계, 마지막 3단계는 HATEOAS를 적용한 단계입니다.
    - 엄밀히 따지면 restful api라고 작성된 것 대부분이 2단계에 머물러 있으므로 Restful API라기 보다는 HTTP API라고 불러야 합니다.
    - 하지만 HATEOAS까지 적용하려면 개발 속도가 저하될 수 있으므로, 팀원 모두가 HATEOAS에 익숙하지 않다면 적당히 타협해서 2단계까지만 사용해도 충분하다고 생각합니다.

</details>

