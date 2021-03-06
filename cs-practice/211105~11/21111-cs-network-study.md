# TCP/UDP의 장단점을 말해주세요.

TCP(Transmission Control Protocol) 연결형 서비스로 3-way handshaking 과정을 통해 연결을 설정합니다. 
 그렇기 때문에 높은 신뢰성을 보장하지만 속도가 비교적 느리다는 단점이 있습니다.

UDP(User Datagram Protocol)는 비연결형 서비스로 3-way handshaking을 사용하지 않기 때문에 신뢰성이 떨어지는 단점이 있습니다. 하지만 수신 여부를 확인하지 않기 때문에 속도가 빠릅니다.
TCP는 신뢰성이 중요한 파일 교환과 같은 경우에 쓰이고 UDP는 실시간성이 중요한 스트리밍에 자주 사용됩니다.

# IPv4와 IPv6의 특징을 말해주세요.
## IPv6
IPv4의 한계인 주소 표현의 제약으로 인해 주소고갈, 멀티미디어서비스 대응 미약을 고려하여 IETF의 IPNG WG에서 표준화 시킨 차세대 인터넷 프로토콜
*	확장된 주소 공간: 128비트 주소체계를 사용해서 IPv4의 주소부족 해결
*	새로운 헤더 포맷: 헤더를 고정 길이로 변경
*	향상된 서비스의 지원
*	보안 기능: IPv4에서의 보안은 IPSec 보안 관련 프로토콜을 별도로 설치해야하지만, IPv6에서는 프로토콜 내에 보안관련 기능을 탑재할 수 있도록 설계 
*	주소 자동설정

## IPv4
인터넷 프로토콜의 4번째 판이며, 전 세계적으로 사용된 첫 번째 인터넷 프로토콜이다. 과거에 인터넷에서 사용되는 유일한 프로토콜이였으나 오늘날에는 IPv6가 대중화되었습니다.

# HTTP vs HTTPS의 차이점을 말해주세요
HTTP(Hypertext Transfer Protocol)는 서로 다른 시스템들 사이에서 통신을 주고받게 해주는 가장 기초적인 프로토콜이며, 평문 데이터를 전송하는 프로토콜이기 때문에, HTTP로 비밀번호나 주민번호 등을 주고 받으면 제3자에 의해 조회될 수 있습니다. 

이러한 HTTP에 암호화가 추가된 프로토콜이 HTTPS(Hypertext Transfer Protocol Secure)입니다. https 프로토콜은 ssl(보안 소켓 계층)을 사용하며, ssl은 서버와 브라우저 사이에 안전하게 암호화된 연결을 만들 수 있게 도와주고 서버 브라우저가 민감한 정보를 주고받을 때 이것이 도난 당하는 것을 막아줍니다

# 웹 동작의 방식 간단히 말해보세요
1.  사용자가 브라우저에 URL을 입력
2.	브라우저는 DNS를 통해 서버의 진짜 주소를 찾음
3.	HTTP 프로토콜을 사용하여 HTTP 요청 메세지를 생성함
4.	TCP/IP 연결을 통해 HTTP요청이 서버로 전송됨
5.	서버는 HTTP 프로토콜을 활용해 HTTP 응답 메세지를 생성함
6.	TCP/IP 연결을 통해 요청한 컴퓨터로 전송
7.	도착한 HTTP 응답 메세지는 웹페이지 데이터로 변환되고, 웹 브라우저에 의해 출력되어 사용자가 볼 수 있게 됨

# 공인 IP와 사설 IP 차이를 말해주세요
## 공인 IP
*	전세계에서 유일한 IP로 ISP(인터넷 서비스 공급자)가 제공하는 IP주소
*	외부에 공개되어 있기 때문에 인터넷에 연결된 다른 장비로부터 접근이 가능하다.
*	그에 따라 방화벽 등과 같은 보안 설정을 해주어야 한다.

## 사설 IP
*	어떤 네트워크 안에서 사용되는 IP주소
*	IPV4의 부족으로 인해 모든 네트워크가 공인 IP를 사용하는 것이 불가능하기 때문에 네트워크 안에서 라우터를 통해 할당받는 가상의 주소이다.
*	별도의 설정 없이는 외부에서 접근이 불가능하다


