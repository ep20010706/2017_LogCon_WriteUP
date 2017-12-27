# #6. [200]소프라노 도메인
문제:
www.teamlog.kr의 최상위 도메인은?

풀이:
최상위 도메인(Top-level domain, TLD)은 인터넷에서 도메인 네임의 가장 마지막 부분을 말한다.
예를 들어 londev.tistory.com 의 최상위 도메인은 .com이다.
그러므로 www.teamlog.kr 의 최상위 도메인은 .kr이다.
Flag는 .kr

# #7. [400]역사적 고전속으로
문제:
새로운 기능과 프로토콜이 개발이 되었을 때 그 프로토콜이 기존의 하드웨어를 고려하지 않았다면 그것을 이용하기 위해선 새로운 프로토콜을 지원하는 새로운 하드웨어가 필요하다.
이러한 수고를 덜기 위해 미리 내장된 지식 없이 새로운 지식을 프로그래밍 하여 사용할 수 있도록 Cisco에서 개발한 칩의 이름은?

풀이:
이 문제는 일반적으로 구글링을 해도 잘 나오지 않았다. 운영진 측에서도 구글링을 통해서 해결할 수 있는 문제 중 가장 어려운 문제였고 나를 제외하곤 푼 사람이 거의 없었던 걸로 기억한다.
(실망스럽게도 이 문제에 대한 답안이 유출되어 일부 참가자가 불이익을 받았었던 것으로 기억한다)
(참고로 4100점을 맞아 중학생 1등을 한 참가자도 이 문제는 못 맞췄던 것 같다.)
나는 영어로도 찾아보고 형태소들을 다 변형하여 일일히 구글링하는 등 여러가지 시도를 해보았으나 답은 나오지 않았다.
엄청난 난이도로 정답자가 나오지 않자, 운영진 측에서는 공지를 통해 정답이 언더바를 포함하여 25자라는 힌트를 주었고 나는 다시 한번 도전하게 만들었다.
이미지 검색 중 UADP라는 Cisco 칩이 있다는 것을 확인했는데 약자를 확인해보니 Unified Access Data Plane 이였고, 글자수가 정확히 25자였다.
답안을 제출해봤는데, 결과는 놀라웠다! 나는 킬러문제를 맞춘 것이다!
Flag는 unified_access_data_plane이다.
[Cisco 문서에서는 UADP (Unified Access Dataplane)를 소프트웨어 유연성을 갖춘 하드웨어 성능을 제공하며 많은 혁신적인 기능을 제공하고, ASIC라 부를 수도 있으며, 유연한 포워딩 엔진과 유선 및 무선 트래픽의 완벽한 통합 기능이라 정의되어있다.]
[Cisco 문서: https://goo.gl/R3XUp4]

# #8. [300]달리는-구성: clock_rate_64000
문제:
다음은 라우터 R1, R2의 running-config의 일부이다.

```
R1
hostname R1
!
interface Serial0/0/0
ip address 10.10.10.1 255.255.255.252
clock rate 64000
!
interface Serial0/0/1
no ip address
clock rate 2000000
shutdown
```

```
R2
Hostname R2
interface Serial0/0/0
ip address 10.10.10.2 255.255.255.252
clock rate 64000
!
interface Serial0/0/1
no ip address
clock rate 2000000
shutdown
```

R1에서 10.10.10.2로 ping테스트를 시행한 결과는 다음과 같다.
Sending 5, 100-byte ICMP Echos to 10.10.10.2, timeout is 2 seconds:
!!!!!
Success rate is 100 percent (5/5), round-trip min/avg/max = 1/7/21 ms

R1의 Serial0/0/0과 R2의 Serial0/0/0이 서로 직접 연결되어 있지 않은 이유를 알 수 있는 부분의 행 전체를 R1의 running-config 또는 ping테스트 결과에서 찾으시오.

풀이:
이건 답이 없는 것 같은데 답이 있다... 그래도 답이 제시한 세팅이나 핑 테스트 결과에 있다니 위에서부터 한줄 한줄 복사해서 답안 제출을 시도한 결과 ```clock rate 64000```가 정답이라는 결과를 도출해냈다.
Flag는 clock_rate_64000이다.

9. [200]위장변장간장: spf
문제:
메일 발송자 정보를 미리 DNS에 등록해놓고, 받은 메일에 개하 DNS질의를 하는 것으로 발송자를 위조하여 메일을 보내는 공격을 예방하는 인증기술 이름은?

풀이:
https://www.kisarbl.or.kr/whiteip/whiteip_tutorial2.jsp 를 참고하면 메일서버등록제(SPF: Sender Policy Framework)는 메일서버 정보를 사전에 DNS에 공개 등록함으로써 수신자로 하여금 이메일에 표시된 발송자 정보가 실제 메일서버의 정보와 일치하는지를 확인할 수 있도록 하는 인증기술이라 나와있다.
Flag는 spf다

10. [100]잠입작전: apt-get_install_tightvncserver
문제:
친구가 학원에 가있는 틈을 타 친구네 집에 원격접속 설정을 해둬서 친구를 골려 주려는 계획을 가지고 친구네 집에 잠입한 성윤이는 친구네 집 컴퓨터의 OS가 Ubuntu인 것을 보고 당황하고 말았다.
빠르게 원격접속 설정을 하지 않으면 친구가 돌아오고 만다!
TightVNC를 이용하여 원격접속을 하려는 성윤이는 급한 나머지 그만 설치 명령어를 기억해내지 못하고 있다.

TightVNC 설치 명령어를 알려줘서 성윤이를 도와라

풀이:
처음엔 ```yum_install_-y_tigervnc-server```로 시도했으나 정답이 아니라 해서 ```yum_install_tigervnc-server```로 했더니 또 오답이라 해서 운영진측에 물어봤더니 해당 문제에 오류가 있음을 확인하여 출제자와 조율하여 답을 수정했다고 하였다.
그리고 ```apt-get_install_tightvncserver```로 시도했더니 맞췄다.
Flag는 ```apt-get_install_tightvncserver```이다.
