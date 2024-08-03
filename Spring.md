





------------------
<details>
  <summary><h1> Security </h1></summary>

  <details>
    <summary><h4> RefreshToken을 저장하기 위해 RDB대신 Redis를 사용한 이유가 무엇인가요? <h3></summary>
  
  - JWT를 사용하면 클라이언트에 Access Token이 노출된다는 단점이 존재합니다.
  - 이를 보완하기 위해서 Access Token의 유효시간을 짧게 설정하여 노출된 토큰의 재사용을 방지하고, RefreshToken을 통해 Access Token을 재발급 받게 하는 방식을 주로 사용합니다.
  - 따라서 AccessToken의 짧은 유효시간 때문에 Refresh Token에 대한 접근이 많을 수 밖에 없는데, RDB에서 Refresh Token을 관리한다면 서버의 다른 비즈니스 로직에 영향을 미칠 수 있기 때문에 Redis에서 관리했습니다.
  - 추가적으로 RDB를 사용한다면 Refresh Token의 유효기간이 지났을 때 Delete 쿼리를 날려줘야 하지만, Redis에서는 만료 시간을 설정해두면 자동으로 삭제할 수 있어서 시스템의 부하를 줄일 수 있습니다.
  
  </details>

</details>
