# ✏️Peer와 socket


## 👩🏻‍🎓PEER(피어)
- peer :[사전적 의미]:또래 혹은 같은편       
![그림2](https://user-images.githubusercontent.com/88940298/147638245-885bd99d-0ff9-400a-bb32-14af75c73c64.png)

블록체인의 가장 핵심 중에 하나는 탈 중앙화이다. 비슷한 사례로 MP3 서비스의 혁명 "소리바다" 이다. 소리바다는 사람들끼리 직접 연결을 시켜서 MP3를 공유하던 서비스이다. 최근에는 토렌트(torrent) 같은 서비스가 나왔지만 2000년대 초에는 소리바다가 P2P 서비스의 최고였다. 즉 P2P는 사람과 사람을 직접 연결하는 기술이다. 블록체인은 일명 CS 구조라고 하는 Client-Server를 채택하지 않는다. 이미 Server라는 말이 "중앙"화라는 말을 의미할 수 있기 때문이다. 물론 P2P도 다른 의미로 CS를 보여줄 수 있다. 예를 들어 사람과 사람 간의 연결을 하더라도 소리바다처럼 누군가가 서버가 되어서 자료를 공유하고 누군가는 클라이언트가 되어서 서비스를 이용하는 역할이 될 수 있기 때문이다. 그러나 일반적인 중앙에 사양이 매우 좋은 서버(Server)에 다중의 클라이언트(Client)가 붙는 구조를 CS 구조라고 하고, 블록체인은 CS보다 P2P를 지향한다.

![그림4](https://user-images.githubusercontent.com/88940298/147638086-1ecfe1bc-c312-4505-b0f9-a35743a8ed80.png)


- Public Blockchain(퍼블릭 블록체인) Similar to Pure P2P

- Private Blockchain(프라이빗 블록체인) Similar to Hybrid P2P

- Consortium Blockchain(컨소시움 블록체인) Similar to Super peer


### 😆P2P 의 장점
- 자유로움:자유롭기 떄문에 더많은 개발자들이 참여 할수 있으며 또한 자유롭기 떄문에 참여를 하는사람들이게 보상을 주면 cs보다 안정적인 서비스를 보여 줄 수 있다
- 구축해 놓으면 사람들이 알아서 서버를 자청하여 생태계를 구축 ,사람들은 코인을 얻기위해 자발적으로 참여
- 보안능력:모든것을 서로간에 감시,모든컴퓨터가 서버-클라이언트 역활을 하기 때문에 상대방의 컴퓨터를 감시하고 올바른 결론으로 도출
- 잘못된 것을 정정하는 민주주의적:누군가의 컴퓨터가 해킹이 되어 잘못된 연산을 한들 나머지 대다수의 컴퓨터가 올바른 판단을 하게되면 잘못된 컴퓨터를 무시할수 있음 -이기능으로 인해서 탈중앙화 방식으로 돌아감
- 노드들중 장애가 발생하여도 서비스에 지장이 크지 않거나 없는 고가용성 혹 내고장성의 서비스를 기본적으로 보여줌

### 😂P2P 의 단점
- 클라이언트-서버구조는 서버를 운영하는 사람이 존재한다면 언제 어디서든지 서비스를 이용할 수 있고 검증된 데이터를 사용할 수 있습니다.서버의 역활해줄 사람이 없다면 서비스를 당연히 이용할 수 없습니다. 본인이 이용한 만큼 본인도 그 댓가를 지불하게 되는 원리이기 떄문에 댓가를 지불하기 싫은 사람이 많을 수록 점점 서비스의 퀄리티도 죽을 수 있습니다.
- 모든 P2P의 노드들의 연결 속도가 빠르면 모르겠지만, 회선이 느린 노드가 존재할 경우 전체 네트워크의 속도를 저하시킬 수 있는 단점이 존재합니다. CS 구조는 운영하는 사람들이 빠른 회선을 쓴다면, 클라이언트 회선만 속도가 보장될 경우 충분히 빠른 서비스를 이용할 수 있지만 P2P는 그렇지 못합니다

### ‼️Public Blockchain(퍼블릭 블록체인) Similar to Pure P2P
퍼블릭 블록체인(public blockchain)은 권위있는 조직의 승인 없이 누구든지 인터넷에 연결된 PC, 노트북, 스마트폰, 서버, 컴퓨터 채굴기 등 다양한 컴퓨터 장비를 이용하여 블록체인 네트워크에 참여가 가능합니다. 즉 공공 블록체인 또는 개방형 블록체인이라고 합니다
```

특징
퍼블릭 블록체인 네트워크에 참여하는 개별 컴퓨터를 ‘노드(node)’라고 부르는데, 각 노드들은 블록체인에 저장된 데이터를 복사하여 저장하고, 해시 연산을 통해 새로운 블록의 생성에 참여할 수 있는 특징을 지닙니다
```
- 보상:퍼블릭 블록체인의 경우 참여자들의 컴퓨터 사용에 따른 전기료 등 운영비용을 감당할 수 있도록, 암호화폐를 발행하여 보상하며 Transaction fee를 받습니다.
- 장점:많은 사람들이 함께 참여하기 때문에 투명성이 강화된 모델이며, 많은 사람들이 네트워크에 참여할 수록 보안이 강화되어 있습니다.
- 단점: 많은 사람들에 의해 합의가 진행되고 전체 네트워크에 전파하여 동기화 해야하기 때문에 속도가 느리다는 단점이 있습니다. 또한, 참여가 자유롭기 때문에 인증 안된 참여자들도 악의적인 목적을 가진 해커도 퍼블릭 블록체인에 접근이 가능합니다.
- 대표적인 블록체인 : 비트코인, 이더리움, 비트코인캐시, 모네로 등
- 대표적인 합의 알고리즘 : POW(Proof of Work, 작업증명) POS(Proof of Stake, 지분증명) DPOS(Delegated Proof of Stake 위임지분증명) 등   
![1_eWhzhPnLulY94kEeiIGnsQ](https://user-images.githubusercontent.com/88940298/147662132-f8a06140-4559-4a06-b629-56b02b5a84ec.png)

### ‼️Private Blockchain(프라이빗 블록체인) Similar to Hybrid P2P
프라이빗 블록체인(Private blockchain)은 법적 책임을 지는 허가 받은 사람만 블록체인 네트워크에 참여할 수 있는 블록체인입니다. 운영과 참여의 주체가 분명하기 때문에 인센티브 제도인 코인을 발행하여 운영하지 않아도 됩니다.
- 장점:허가받은 소수의 사람들이 참여하기 때문에 기밀성이 강화된 모델이며, 신뢰할 수 있는 사람들만 참여하여 트랜잭션 속도가 빠릅니다.
- 단점: 적은 사람들에 의해 합의가 진행되기 때문에 일부 중앙화가 되어 보안성이 낮아질 수 있습니다.
- 대표적인 블록체인 : Hyper ledger fabric, R3 CORDA 등
- 대표적인 합의 알고리즘 : PBFT(Practical byzantine fault tolerance) 등
- 완전한 프라이빗 블록체인(Fully private blockchain): 하나의 기관 또는 기업 아래서 사용되는 블록체인, 데이터 관리와 검증, 거래내역에 접근하기 위해서는 중앙기관에서 허가를 받아야 가능합니다. 블록체인 기술을 사용하지만 중앙이 힘을 가지고 있고, 그저 분산된 데이터베이스만 갖는 구조로서 현재 전통의 시스템에 블록체인의 보안 검증성의 특징만 가져옵니다.
- 컨소시움 블록체인(consortium blockchain):여러 기관 또는 기업이 하나의 그룹을 이뤄 블록체인 네트워크를 구성하는 구조를 가지고 있습니다. 퍼블릭 프라이빗 블록체인의 성격을 모두 가질 수 있으며, 노드에도 특정 역할을 부여할 수 있는 통제권을 가진 블록체인 네트워크입니다.   
![1_Hkm9ZXiqcgE2tRcEFw8qkA](https://user-images.githubusercontent.com/88940298/147662331-ef5ea20d-e250-4bd6-8d79-51cf6b6dcfdd.png)
#### ⓵프라이빗 블록체인 활용 사례
- 월마트(wallmart) : 실재료의 생산과 유통 과정 전체에 프라이빗 블록체인 기술을 적용하여 실시간으로 위생 상태를 점검할 수 있는 데이터 저장 방식을 도입
해운회사 머스 : IBM 프라이빗 블록체인을 이용한 선박 물류 시스템을 개발하여 서류없이 물건을 옮기고 주문하고 보관, 세관 신고를 처리할 수 있는 물류 시스템 개발
- 삼성 SDS : 중고차 시장에 위조가 불가능한 프라이빗 블록체인 기술을 적용하여 차량의 수리, 사고 상태를 한눈에 학인하고 구입할 수 있는 중고차 이력 서비스 개발 중, 네덜란드 3대 은행의 하나인 ABN AMRO, 삼성SDS는 로테르담 항만공사의 해운물류 사업에 블록체인 기술을 적용하기 위해 자사 블록체인 플랫폼(넥스레저, Nexledger)을 ABN AMRO의 블록체인 플랫폼(코다, Corda)과 연계하는 시범 프로젝트를 내년 2월까지 완료할 계획
- 구글 : deepmind는 블록체인 기술을 활용하여 의료기록을 관리하는 솔루션을 개발하기로 함 구글 deepmind는 verifiable data audit이라고 블리는 의료 기록 관리 솔루션을 개발할 것이며 이는 블록체인 기술을 기반으로 의료 데이터를 관리 할 것이라고 함


### ❗️Consortium Blockchain(컨소시움 블록체인) Similar to Super peer
컨소시엄 블록체인(Consortium Blockchain)은 퍼블릭과 프라이빗 블록체인의 중간 형태로 중앙 관리자에 의해 승인받은 참여자만이 블록 생성에 참여할 수 있는 프라이빗 블록체인과 유사한 개념이라고 할 수 있습니다.
하지만 둘을 구분 짓자면 프라이빗 블록체인은 네트워크에 참여할 수 있는 사람들을 제한하여 하나의 기관에서 독자적으로 사용하는 블록체인 망을 구성하는 반면, 컨소시엄 블록체인은 같은 목적을 가지고 있는 여러 기관이 하나의 컨소시엄을 구성하여 공정성과 확장성을 보완하였다. 따라서 다수 참여자의 협의가 필요한 분야에서는 컨소시엄 블록체인이 프라이빗 블록체인보다 효과적,프라이빗 블록체인에서 탈 중앙화를 더하려는 형태입니다.

- 장점: 개발사는 게임 개발에 집중을 할 수 있습니다. 브릴라이트 플랫폼이 제공하는 SDK를 사용하면 따로 블록체인에 신경을 쓸 필요가 없고, 게이머들의 계정이나 아이템 관리 등의 업무에서 해방될 수 있습니다.
- 장점2:여러 개발사와 협력을 할 수 있다는 점입니다. 협력이 장점이 되는 이유는 글 서두에 언급한 기술의 발전과 큰 연관이 있습니다. 기하급수적으로 발전하는 기술에 홀로 대처하는 것은 어렵기 때문에 협업이 굉장히 중요한 요소라고 할 수 있습니다.
- 장점3:컨소시엄 블록체인이 주목받는 가장 큰 이유는 플랫폼과 네트워크를 구축·개발하는 데 발생하는 원가를 공유할 수 있기 때문입니다. 또한, 기존에 시간과 비용이 많이 들었던 업무 과정을 저가로 빠르고 효율적으로 처리할 수 있습니다

![img](https://user-images.githubusercontent.com/88940298/147664118-0d51ad79-aa2b-41c5-8114-ae685e93a390.png)


## 👩🏻‍🎓SOKET(소켓)
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
### ⁉️Tranceport Layer
- End Palnt간 신뢰성 있는 데이터 전송을 담당하는 계층
- 신뢰성 : 데이터를 순차적,안정적인 전달
- 전송 : 포트 번호에 해당하는 프로세스에 데이터를 전달
##### 전송계층이 없다면(전송 계층의 중요성)
- 데이터의 순차 전송 원활이 x
- Flow(흐름문제)-원인:송수신자간의 데이터 처리 속도 차이,수신자가 처리할 수 있는 데이터량을 초과
- Congention(혼잡문제) 원인 : 네트워크의 데이터 처리 속도 (ex.라우터),Network가 혼잡할떄
- 결과적으로 데이터의 손실이 발생 !!

###  ⁉️UDP 프로토콜
![2018-02-04-network-tcp-udp-tcpip-3](https://user-images.githubusercontent.com/88940298/147642733-7f5353ec-0c4e-4293-b3d0-942bd039036f.png)


- TCP보다 신뢰성이 떨어지지만 전송속도가 일반적으로 빠른 프로토콜(순차전송x,흐름제어x,혼잡제어x)
- Connectionless (3 way-handshake x)
- Error Detection
- 비교적 데이터의 신뢰성이 중요하지 않을 떄 사용(ex 영상 스트리밍)

#### User Datagram - UDP 프로토콜의 PDU
- 데이터에 UDP헤더 추가
- TCP처럼 데이터를 쪼개지 않음
#### 데이터 전송방식
- 보내면 받음
### ⁉️TCP 프로토콜
![2018-02-04-network-tcp-udp-tcpip-2](https://user-images.githubusercontent.com/88940298/147642803-5968ffdd-5a58-4b26-b72c-30ad96082620.png)


- 신뢰성 있는 데이터 통신을 가능하게 해주는 프로토콜
- 특징: Connection 연결(3 way-handshake)-양방향 통신
- 데이터의 순차 전송을 보장
- Flow Control(흐름제어)
- Congention Control (혼잡제어)
- Error Detection(오류 감지)
#### ⓵Segment(세그먼트) -TCP 프로토콜의 pdu
- 프로토콜 안에서 처리되고 움직이는 데이터의 단위
- 데이터 받은것을 잘라서 TCP Header를 추가한것
#### ②TCP Header
- TCP 연결 제어 및 데이터 관리
#### ③TCP의 3-Way handshake (Connection연결)
- SYN.비트를 1로 설정해 패킷 송신
- SYN.ACK비트를 1로 설정해 패킷 송신
- ACK 비트를 1로 설정해 패킷 송진
#### ④TCP의 데이터 전송 방식
- 1.client가 패킷송신
- 2.Server에서 Ack송신
- 3.ACK 수신하지 못하면 재전송
#### ⑤4.way-handshake(Connection close)
- 데이터를 전부 송신한 client가 FIN송신
- Server가 ACK송신
- Server에서 남은 패킷 송신(일정 시간 대기)
- Server가 FIN송신
- Client가 ACK송신

![226CBB4852BBDDB70B](https://user-images.githubusercontent.com/88940298/147642647-8e405a70-542d-4416-a53d-5593c50ecef1.jpeg)

#### ‼️😅TCP의 문제점
- 전송의 신뢰성은 보장하지만..
- 매번 Connection을 연결해서 시간 손실 발생(3-Way handshake)
- 패킷을 조금만 손실해도 재전송

### ⁉️웹소켓 (WebScoket)
WebSocket은 ws 프로토콜을 기반으로 클라이언트와 서버 사이에 지속적인 완전 양방향 연결 스트림을 만들어 주는 기술입니다. 
HTTP통신과 호환이 되며, 처음 접속시 http통신과 handshake가 이루어진다. handshake는 처음 접속 때 한번만 이루어진다.

![991](https://user-images.githubusercontent.com/89236248/147659757-78b64663-c461-432e-ac01-6be43680cde3.png)


### ⁉️웹소켓 (WebScoket)과 TCP/IP 소켓의 차이점은?
- 웹 소켓은 HTTP 레이어에서 작동하는 소켓으로 TCP/IP 소켓의 레이어가 다르다. (RFC-6455)
- IP, PORT를 통해서 통신한다는 점에서는 비슷하다.
- 기존 HTTP 통신의 경우에는 단방향 통신으로 실시간 통신을 하기 위해서는 실시간처럼 보이는 방식을 사용한다.(Polling 방식)
- 이후 실제로 실시간 양방향 통신이 가능한 웹 소켓은 2011년 국제 인터넷 표준화 기구(IETF)에서 RFC 6455로 표준화가 되었다.
- 웹 소켓의 프로토콜 표시는 WS(WebSocket)과 WSS(WebSocket Secure)이 있다.
- 웹소켓을 지원하지 않는 브라우저 등이 있기 있지만 현재는 거의 모든 벤더사에서 웹 소켓을 지원하고 있다.

### ⁉️소켓 통신할때 필요한 주요함수

1. socket(int domain, int type, int protocol)
소켓을 만드는데 바로 이 함수를 사용합니다. 소켓 역시 파일로 다루어지기 때문에 반환값은 파일디스크립터입니다. 만약 소켓을 여는데 실패했다면 -1을 리턴합니다.

2. connect(int fd, struct sockaddr *remote_host, socklen_t addr_length)
원격 호스트(원격 컴퓨터)와 연결하는 함수입니다. 연결된 정보는 remote_host에 저장됩니다. 성공시 0, 오류시 -1을 반환합니다.

3. bind(int fd, struct sockaddr *local_addr, socklen_t addr_length)
소켓을 바인딩합니다. 이렇게 생각하면 됩니다. 지금 fd로 넘겨지는 소켓과 이 프로세스와 묶는다(bind)라고 생각하시면 됩니다. 그래서 해당 프로세스는 소켓을 통해 다른 컴퓨터로부터 연결을 받아들일 수 있습니다.

4. listen(int fd, int backlog_queue_size)
 소켓을 통해 들어오는 연결을 듣습니다. backlog_queue_size만큼 연결 요청을 큐에 넣습니다. 성공시 0, 오류시 -1을 반환합니다.

5. accept(int fd, sockaddr *remote_host, socklen_t *addr_length)
어떤 컴퓨터에서 이 컴퓨터로 연결할때 연결을 받아들입니다. 함수 이름이 말해주고 있죠.
연결된 원격 컴퓨터의 정보는 remote_host에 저장됩니다. 오류시에 -1을 반환합니다.

6. send(int fd, void* buffer, size_t n, int flags)
buffer를 소켓 파일 디스크립터인 fd로 전송합니다. 보낸 바이트수를 반환하며 실패시 -1을 반환합니다.

7. recv(int fd, void* buffer, size_t n, int flags)
send함수와 사용법이 거의 비슷합니다. n바이트를 buffer로 읽습니다. 성공시 받은 바이트수를 반환하며 실패시 -1을 반환합니다.
웹소켓의 통신 TCP 80포트 를 사용하면서 HTTP 프로토콜과 호환되며, 웹브라우저와 서버간 통신을 가능하게 해준다.

### ⁉️웹소켓 서버 만들기

```
//server.js
const WebSocket = require('ws');

const ws = new WebSocket.Server({ port: 8080 });

console.log("Server Started");


ws.on('connection', (wss) => {

  console.log("A new Client Connected")

  wss.send('Welcome to the Server!');


  wss.on('message', (message) => {

    console.log(`Server Received: ${message}`);


    wss.send('Got your Message: ' + message);

  });

});
```

```
//client.js
const socket = new WebSocket('ws://localhost:8080');

socket.addEventListener('open', () => {

    console.log('Connected to the Server!');

});


socket.addEventListener('message', (msg) => {

    console.log(`Client Received: ${msg.data}`);

});


const sendMsg = () => {

    socket.send('메세지입력');
}
```


 
