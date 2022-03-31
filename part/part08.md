# PART 08 라우팅 프로토콜과의 한판

### 1. RIP라는 라우팅 프로토콜에 대한 이야기

- RIP 라우팅 프로토콜(Routing Information Protocol)
  - 다이내믹 라우팅 프로토콜
  - 내부용 라우팅 프로토콜(Interior Gateway Protocol, IGP)
  - Distance(거리) Vector(방향) 라우팅 프로토콜
  - RIP 라우팅 프로토콜에서 라우터가 좋은 길을 결정하는 기준이 되는 요소 -> 홉(Hop) 카운트
  - RIP 라우팅 프로토콜에서 최대한 갈 수 있는 홉 카운트의 거리 -> 15개, 16개부터는 도착이 불가능
  - RIP의 디폴트 라우팅 업데이트 주기 -> 30초

### 2. RIP와 함께 춤을?

### 3. Distance - Vector 라우팅 알고리즘에서의 문제점과 해결책

### 4. IGRP 라우팅 프로토콜

- IGRP(Interior Gateway Routing Protocol)
  - 다이내믹 라우팅 프로토콜
  - 내부용 라우팅 프로토콜(Interior Gateway Protocol, IGP)
  - Distance(거리) Vector(방향) 라우팅 프로토콜
  - IGRP는 RIP와 달리 시스코 라우터에서만 사용 가능
  - IGRP는 다섯 가지 요인을 가지고 가장 좋은 경로를 선택
  - IGRP 90초에 한번 라우팅 테이블의 업데이트

### 5. OSPF 라우팅 프로토콜

- OSPF(Open Shortest Path First) 라우팅 프로토콜
