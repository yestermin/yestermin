# 15. CDN — 여러 도시에 미리 세운 물류창고

---

같은 해외 동영상 사이트인데, 어떤 영상은 끊김 없이 나오고 어떤 영상은 유독 버퍼링이 걸리는 걸 이상하게 여긴 적 있으신지.

CDN은 원본 서버에 있는 콘텐츠를 세계 여러 지점의 서버에 미리 복사해 두고, 사용자와 가장 가까운 곳에서 내려받게 해주는 네트워크다. 콘텐츠 전송 네트워크라는 이름 그대로다.

## 여러 도시에 미리 세운 물류창고

본사 창고가 미국 한 곳에만 있는 유통회사를 생각해보자. 한국에서 주문이 들어오면 그 물건은 태평양을 건너와야 한다. 오래 걸린다. 이 회사가 서울과 도쿄와 프랑크푸르트에도 작은 창고를 두고, 잘 나가는 물건을 미리 갖다 놓으면 얘기가 달라진다. 한국 주문은 서울 창고에서 바로 나간다. CDN이 이 방식이다. 원본은 한 곳에 있어도, 자주 찾는 콘텐츠는 세계 곳곳의 창고(엣지 서버라 부른다)에 미리 복사해둔다.

앞서 캐시 편에서 이 동네 조리대 이야기를 잠깐 꺼냈는데, CDN은 그 조리대를 나라마다 정식으로 깔아둔 큰 물류망이라고 보면 된다. 캐시가 "가까운 곳에 사본을 둔다"는 원리 자체라면, CDN은 그 원리를 세계 규모로 깐 실제 인프라에 가깝다.

창고가 여럿이면 본사 창고에도 좋은 점이 있다. 웬만한 주문은 지역 창고에서 다 소화하니, 본사 창고는 정작 중요한 순간에 여유를 갖는다. 갑자기 주문이 몰려도 지역 창고들이 나눠 받으니 본사가 마비되는 일이 줄어든다. 갑작스러운 접속 폭주를 견디는 데 CDN이 쓰이는 이유다.

## 실제로 굴러가는 자리

동영상 스트리밍 서비스가 끊김 없이 재생되는 데는 가까운 지역 서버에서 영상을 받아오는 구조가 큰 몫을 한다. 큰 웹사이트의 이미지나 로고, 스타일 파일도 대개 CDN을 거쳐 내려온다. 새 제품 발표나 티켓 오픈처럼 순간적으로 접속이 몰리는 순간에도 CDN이 트래픽을 지역별로 나눠 받아, 원본 서버가 그대로 무너지는 걸 막아준다.

## 흔히 잘못 아는 것

CDN을 쓰면 항상 더 빠르다고 여기기 쉬운데, 원본 콘텐츠가 방금 바뀐 직후라면 지역 창고에는 아직 옛날 사본이 남아 있을 수 있다. 이 경우 갱신된 내용이 퍼지는 데 시간이 조금 걸린다. 캐시에서 봤던 그 어긋남이 여기서도 그대로 나타난다.

CDN이 콘텐츠를 영구히 보관해준다고 생각하는 것도 오해다. 지역 창고의 사본은 임시 보관이라, 오래 안 찾으면 밀려나고 사라진다. 진짜 원본은 여전히 본사 창고, 즉 원 서버에 있다.

모든 콘텐츠에 CDN이 똑같이 유리한 것도 아니다. 로그인한 사람마다 내용이 다른 개인화된 화면 같은 건 미리 복사해둘 수가 없다. CDN은 누구에게나 똑같이 나가는 콘텐츠에서 특히 힘을 발휘한다.

## 함께 알아두면 좋은 말

| 용어 | 뜻 |
| --- | --- |
| 캐시 | 가까운 곳에 사본을 둬 빨리 꺼내 쓰는 원리 자체 |
| 오리진 서버 | 진짜 원본이 있는 본사 창고 |
| 엣지 서버 | 사용자와 가까운 곳에 놓인 지역 창고 |
| 레이턴시 | 요청하고 응답받기까지 걸리는 시간. 거리가 멀수록 늘어난다 |

본사에서 아무리 좋은 물건을 만들어도, 그걸 손님 앞까지 가져다주는 거리가 길면 소용이 없다. CDN이 파는 건 결국 콘텐츠가 아니라 거리다.

---

![대표 이미지](images/15_CDN/15_CDN_1_cover.png)

본문에 그림이 들어가면 좋을 자리는 아래와 같다. 실제 이미지는 아직 넣지 않았다.

〔이미지 자리 — 세계지도 위에 본사 창고 하나와 여러 도시의 작은 지역 창고들이 표시되고, 상품이 가까운 창고에서 바로 나가는 경로〕

〔이미지 자리 — 접속이 몰린 순간, 여러 지역 창고가 나눠 받아 본사 창고가 무너지지 않는 모습〕

〔이미지 자리 — 본사 창고의 물건은 이미 새 버전인데 지역 창고 선반엔 옛날 버전이 아직 남아 있는 장면〕

## 이미지 생성 프롬프트

1. 대표 이미지: A flat vector world map with one large central warehouse and several small local warehouse icons in different cities, thin delivery lines connecting the central warehouse to each local one, flat vector illustration style, a simple everyday-object metaphor explaining a tech concept, minimal color palette, no text in the image, 16:9 composition.
2. 이미지 자리 1: A flat vector illustration zoomed into one local city warehouse quickly handing a package straight to a nearby customer at the door, with a faint dotted line in the background showing the much longer route it would have taken from a distant central warehouse, flat vector illustration style, a simple everyday-object metaphor explaining a tech concept, minimal color palette, no text in the image, 4:3 composition.
3. 이미지 자리 2: A flat vector scene of a sudden surge of delivery trucks being split evenly among several small regional warehouses instead of all converging on one overwhelmed central warehouse, flat vector illustration style, a simple everyday-object metaphor explaining a tech concept, minimal color palette, no text in the image, 4:3 composition.
4. 이미지 자리 3: A flat vector split scene, the central warehouse shelf showing a freshly updated product box, while a distant regional warehouse shelf still shows the old version of the same box, flat vector illustration style, a simple everyday-object metaphor explaining a tech concept, minimal color palette, no text in the image, 4:3 composition.
