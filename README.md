# spring-cloud-config
Sample Of spring-cloud-config

## config-server
* @EnableConfigServer 어노테이션을 선언해야 한다.
* server에 등록한 client의 config 확인
  * http://localhost:8888/config-client/{default | dev |...}

## config-client
* @RefreshScope
  * 사용자 정의 스프링 프로퍼티만 다시 로드한다.
  * http://<config-client>:port/actuator/refresh 를 호출해서 갱신한다.