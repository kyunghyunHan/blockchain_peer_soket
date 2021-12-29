# Peer와 socket


## 👩🏻‍🎓PEER(피어)
- peer :[사전적 의미]:또래 혹은 같은편       
![그림2](https://user-images.githubusercontent.com/88940298/147638245-885bd99d-0ff9-400a-bb32-14af75c73c64.png)

블록체인의 가장 핵심 중에 하나는 탈 중앙화이다. 비슷한 사례로 MP3 서비스의 혁명 "소리바다" 이다. 소리바다는 사람들끼리 직접 연결을 시켜서 MP3를 공유하던 서비스이다. 최근에는 토렌트(torrent) 같은 서비스가 나왔지만 2000년대 초에는 소리바다가 P2P 서비스의 최고였다. 즉 P2P는 사람과 사람을 직접 연결하는 기술이다. 블록체인은 일명 CS 구조라고 하는 Client-Server를 채택하지 않는다. 이미 Server라는 말이 "중앙"화라는 말을 의미할 수 있기 때문이다. 물론 P2P도 다른 의미로 CS를 보여줄 수 있다. 예를 들어 사람과 사람 간의 연결을 하더라도 소리바다처럼 누군가가 서버가 되어서 자료를 공유하고 누군가는 클라이언트가 되어서 서비스를 이용하는 역할이 될 수 있기 때문이다. 그러나 일반적인 중앙에 사양이 매우 좋은 서버(Server)에 다중의 클라이언트(Client)가 붙는 구조를 CS 구조라고 하고, 블록체인은 CS보다 P2P를 지향한다.

![그림4](https://user-images.githubusercontent.com/88940298/147638086-1ecfe1bc-c312-4505-b0f9-a35743a8ed80.png)


- Public Blockchain(퍼블릭 블록체인) Similar to Pure P2P

- Private Blockchain(프라이빗 블록체인) Similar to Hybrid P2P

- Consortium Blockchain(컨소시움 블록체인) Similar to Super peer
## SOKET(소켓)
소켓(Socket)이란 네트워크상에서 서버와 클라이언트 두개의 프로그램이 특정 포트를 통해 양방향 통신이 가능하도록 만들어주는 소프트웨어 장치이다.
오늘날 컴퓨터 간 통신의 대부분은 인터넷 프로토콜을 기반으로 하고 있으므로, 대부분의 네트워크 소켓은 인터넷 소켓이다. 네트워크 통신을 위한 프로그램들은 소켓을 생성하고, 이 소켓을 통해서 서로 데이터를 교환한다. 소켓은 RFC 147에 기술사항이 정의되어 있다.

인터넷 소켓은 다음과 같은 요소들로 구성되어 있다.
- 인터넷 프로토콜 (TCP, UDP, raw IP)
- 로컬 IP 주소
- 로컬 포트
- 원격 IP 주소
- 원격 포트

인터넷 소켓은 크게 두 개의 타입으로 분류할 수 있다.
- UDP 프로토콜을 사용하는 경우
- TCP 프로토콜을 사용하는 경우
### Tranceport Layer
- End Palnt간 신뢰성 있는 데이터 전송을 담당하는 계층
- 신뢰성 : 데이터를 순차적,안정적인 전달
- 전송 : 포트 번호에 해당하는 프로세스에 데이터를 전달
##### 전송계층이 없다면(전송 계층의 중요성)
- 데이터의 순차 전송 원활이 x
- Flow(흐름문제)-원인:송수신자간의 데이터 처리 속도 차이,수신자가 처리할 수 있는 데이터량을 초과
- Congention(혼잡문제) 원인 : 네트워크의 데이터 처리 속도 (ex.라우터),Network가 혼잡할떄
- 결과적으로 데이터의 손실이 발생 !!

###  UDP 프로토콜

### TCP 프로토콜
- 신뢰성 있는 데이터 통신을 가능하게 해주는 프로토콜
- 특징: Connection 연결(3 way-handshake)-양방향 통신
- 데이터의 순차 전송을 보장
- Flow Control(흐름제어)
- Congention Control (혼잡제어)
- Error Detection(오류 감지)
#### Segment(세그먼트) -TCP 프로토콜의 pdu
- 프로토콜 안에서 처리되고 움직이는 데이터의 단위
- 데이터 받은것을 잘라서 TCP Header를 추가한것
#### TCP Header
- TCP 연결 제어 및 데이터 관리
#### TCP의 3-Way handshake (Connection연결)
- SYN.비트를 1로 설정해 패킷 송신
- SYN.ACK비트를 1로 설정해 패킷 송신
- ACK 비트를 1로 설정해 패킷 송진
#### TCP의 데이터 전송 방식
- 1.client가 패킷송신
- 2.Server에서 Ack송신
- 3.ACK 수신하지 못하면 재전송
#### 4.way-handshake(Connection close)
- 데이터를 전부 송신한 client가 FIN송신
- Server가 ACK송신
- Server에서 남은 패킷 송신(일정 시간 대기)
- Server가 FIN송신
- Client가 ACK송신
#### TCP의 문제점
- 전송의 신뢰성은 보장하지만..
- 매번 Connection을 연결해서 시간 손실 발생(3-Way handshake)
- 패킷을 조금만 손실해도 재전송
