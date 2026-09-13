# 12. VPN — 봉인해서 보내는 택배 상자

---

카페 공용 와이파이에 접속할 때마다, 이 신호를 누가 옆에서 들여다보고 있는 건 아닐까 찜찜했던 적 있으신지.

VPN은 인터넷 위에 나만 쓰는 사설 통로를 만들어, 그 안을 오가는 내용을 다른 사람이 못 보게 감싸 보내는 기술이다.

## 겉을 감싼 택배 상자

보통 인터넷 통신은 엽서를 보내는 것과 비슷하다. 중간 우체국 여러 곳을 거치는데, 마음만 먹으면 중간에서 내용을 슬쩍 볼 수 있는 구조다. VPN은 그 엽서를 겉을 알아볼 수 없는 봉인 상자에 넣어 보낸다. 상자를 나르는 사람(중간의 통신 경로)은 상자가 오간다는 사실은 알아도 안에 뭐가 들었는지는 못 본다.

이 상자는 지정된 배송 업체(VPN 서버)를 거쳐 목적지로 간다. 그래서 상자를 받는 쪽에서 보면 발신지가 원래 있던 곳이 아니라 그 배송 업체 창고로 보인다. 해외에 있는 VPN 서버를 거치면 그 나라에서 접속한 것처럼 보이는 이유가 이거다. 다만 배송 업체가 상자를 열어볼 마음만 먹으면 열어볼 수 있다는 점은 남는다. 봉인은 중간의 다른 사람들로부터 지켜줄 뿐, 배송 업체 본인으로부터 지켜주지는 못한다.

## 실제로 어떻게 쓰이나

재택근무자가 회사 내부 시스템에 접속할 때 VPN을 켜는 건, 회사 건물 안에 있는 것처럼 위장해 사설 통로로 들어가는 것이다. 해외 출장 중에 국내에서만 되는 서비스를 쓰려고 VPN을 켜는 것도 같은 원리다. 공공 와이파이에서 결제나 로그인을 할 때 VPN을 권하는 이유도, 옆에서 신호를 가로채는 위험을 줄이기 위해서다.

## 흔히 잘못 아는 것

VPN을 켜면 완전히 익명이 된다고 생각하기 쉬운데, 그 봉인 상자를 나르는 배송 업체, 즉 VPN 서비스 운영사는 원칙적으로 내용을 볼 수 있는 위치에 있다. 어떤 정보를 얼마나 기록하는지는 업체마다 정책이 다르고, 그 정책을 얼마나 지키는지는 이용자가 직접 확인하기 어렵다. 무료 VPN일수록 이 부분을 꼼꼼히 따져봐야 한다는 말이 나오는 이유다.

속도가 항상 빨라진다는 것도 사실과 다르다. 상자를 포장하고 먼 배송 업체를 거치는 과정 자체가 시간을 잡아먹는다. 오히려 평소보다 느려지는 경우가 흔하다. 그리고 VPN은 통로를 감추는 기술일 뿐, 그 통로로 하는 행동을 정당하게 만들어주는 장치는 아니다.

## 함께 알아두면 좋은 말

| 용어 | 뜻 |
| --- | --- |
| 암호화 | 상자 안 내용을 알아볼 수 없게 바꾸는 작업 자체 |
| 프록시 | VPN처럼 우회는 하지만 대체로 감싸는 정도가 약한 방식 |
| 공인 IP | VPN을 거치면 상대에게 보이는 주소가 이걸로 바뀐다 |
| 접속 로그 | VPN 업체가 남길 수도, 안 남길 수도 있는 이용 기록 |

봉인 상자는 나르는 사람을 못 믿을 때 유용하다. 그런데 그 상자를 대신 날라주는 배송 업체를 얼마나 믿을 것인가는, VPN을 켜는 순간 슬쩍 넘어가기 쉬운 질문이다.

---

![대표 이미지](images/12_VPN/12_VPN_1_cover.png)

본문에 그림이 들어가면 좋을 자리는 아래와 같다. 실제 이미지는 아직 넣지 않았다.

〔이미지 자리 — 평범한 엽서가 오가는 길과, 봉인된 상자가 오가는 길을 나란히 대비한 장면〕

〔이미지 자리 — 봉인 상자가 해외의 배송 업체 창고를 거쳐 다시 목적지로 향하는 경로도〕

〔이미지 자리 — 카페에서 노트북을 쓰는 사람 주위로, 옆 테이블에서 훔쳐보는 그림자가 봉인 상자에 막혀 튕겨나가는 모습〕

## 이미지 생성 프롬프트

1. 대표 이미지: A flat illustration split into two halves — on the left an open postcard traveling through several hands, on the right a sealed opaque parcel box traveling through the same path untouched, flat vector illustration style, a simple everyday-object metaphor explaining a tech concept, minimal color palette, no text in the image, 16:9 composition.
2. 이미지 자리 1: A flat vector map-style illustration of a sealed parcel box traveling from one country through a distant warehouse building before continuing on to its final destination, flat vector illustration style, a simple everyday-object metaphor explaining a tech concept, minimal color palette, no text in the image, 4:3 composition.
3. 이미지 자리 2: A flat vector scene of a person using a laptop in a cafe, with a shadowy figure at a nearby table trying to peek but being blocked by a glowing sealed box icon around the laptop's signal, flat vector illustration style, a simple everyday-object metaphor explaining a tech concept, minimal color palette, no text in the image, 4:3 composition.
