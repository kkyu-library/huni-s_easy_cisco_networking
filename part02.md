# PART 02 네트워크와 케이블, 그리고 친구들

### 1. LAN(Local Area Network)이란?
- LAN(Local Area Network) - 어느 한정된 공간의 네트워크 구축
- WAN(Wide Area Network) - 멀리 떨어진 곳과의 네트워크 구축

### 2. 이더넷은 인터넷의 친구?
- 이너넷(Ethernet) - 네트워킹의 한 방식, 즉 네트워크를 만드는 방법 중 하나
- 이너넷 방식의 특징
  - 지금 우리나라에서 사용하고 있는 네트워킹 방식
  - CSMA/CD 프로토콜 사용
- CSMA/CD(Carrier Sense Multiple Access/Coolision Detection) - 대충 알아서 눈치껏 통신하자
  - 이더넷 환경에서 통신을 하고 싶은 PC나 서버는 네트워크상에 통신이 일어나고 있는지를 확인한다. -> Carrier Sense (Carrier - 네트워크상에 나타나는 신호)
  - Carrier가 감지되면 대기한다. 그러다가 통신(Carrier)이 없어지면 통신한다.
  - 만약 Carrier가 없는 네트워크상에 동시에 데이터를 실어 보내는 경우가 발생할 수 있다. -> Multiple Access(다중 접근)
  - Multiple Access의 경우 충돌(Collision)이 발생! 따라서 이더넷에서는 데이터를 네트워크에 보내고 충돌이 발생했는지 점검해야한다. -> Collision Detection(충돌 감지)
  - 충돌을 감지하면 랜덤한 시간 후에 다시 보낸다. (15번까지 반복) 

### 3. 그럼 토큰링(TokenRing)은요?
- 오직 한 PC, 즉 토큰을 가진 PC만이 통신하는 네트워킹 방식
- 통신을 완료하면 다음 컴퓨터로 토큰을 건넨다.
- 장점
  - 충돌이 발생하지 않는다.
  - 네트워크 성능을 예측하기 쉽다.
- 단점
  - 차례를 기다려야 한다.   

### 4. UTP 케이블만이라도 제대로 알아볼까요?
- UTP(Unshielded Twiseted Pair)
  - 주로 우리가 사용하는 케이블   
- STP(Shielded Twiseted Pair)
  - 케이블의 주위를 절연체로 감싸서 보호
  - UTP보다 비싸고 성능 좋음
  - 주로 토큰링쪽에 많이 쓰임
- 카테고리 1: 주로 전화망에 사용, 따라서 데이터 전송요으로 부적합
- 카테고리 2: 데이터를 최대 4Mbps의 속도로 전송하는 케이블
- 카테고리 3: 10 Base T 네트워크에 사용되는 케이블. 최대 10Mbps
- 카테고리 4: 토큰링 네트워크에서 사용. 최대 16Mps
- 카테고리 5: 최대 100Mbps. 기가비트도 가능
- 카테고리 6: 기가비트 이상의 속도에 적합한 케이블. 
- 카테고리 7: 10Gbps 속도 이상의 적합한 케이블..   

### 5. 케이블, 이 정도만 알면…
- 10 Base T
- 10: 10Mbps 속도를 지원하는 케이블
- Base: 베이스밴드를 지원하는 케이블 (Baseband,디지털 방식 vs Broadband,아날라고 방식)
- T: 케이블의 종류 또는 케이블이 전송할 수 있는 최대 거리 여기서는 UTP

### 6. 맥 어드레스(MAC Address)에 대한 이야기
- MAC(Media Access Control) - 네트워크상에서 서로를 구분하는 주소
- IP 주소를 MAC으로 바꾸는 절차(ARP, Address Resulution Protocol)
- 48bit, 6옥텟(octet) -> 12자리의 16진수 맥어드레스
- 앞에서 6개의 16진수가 벤더, 생성자를 나타내느 코드로, 이 코드를 OUI(Orgnizational Unique Identifier)이라 한다.

### 7. 유니캐스트, 브로드캐스트, 멀티캐스트
### 8. OSI 7 Layer(계층)는 왜 만들어졌나요?
### 9. 컴퓨터는 프로토콜(Protocol)로 말한다
