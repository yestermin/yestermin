# 11. HTTP vs HTTPS — 자물쇠 아이콘이 뜨면 안전하다는 착각

---

주소창에 자물쇠 아이콘이 뜨면 안심하고 로그인 정보를 입력하는 사람이 많다. 그 아이콘이 말해주는 건 이 사이트가 정직하다가 아니라 이 구간의 통신이 암호화되어 있다는 사실뿐이다. 사기 목적으로 만든 사이트도 얼마든지 자물쇠를 달 수 있다. 자물쇠는 봉투가 잠겼다는 뜻이지, 보낸 사람이 좋은 사람이라는 보증서가 아니다.

## 봉투에 넣었나 안 넣었나

HTTP는 브라우저와 서버가 정보를 주고받는 규칙이다. 다만 그 내용을 그대로, 엽서 쓰듯 평문으로 주고받는다. 중간의 통신망을 들여다볼 수 있는 사람이 있다면 아이디와 비밀번호까지 그대로 읽힌다. HTTPS는 그 규칙에 암호화 계층을 얹은 것이다. 같은 내용을 봉투에 넣어 봉인한 다음 보낸다고 보면 된다. 중간에서 가로채도 내용물이 뒤섞인 글자로만 보인다.

이 봉인 작업을 해주는 게 TLS라는 암호화 프로토콜이다. 예전에는 SSL이라 불렀는데 기술이 여러 차례 바뀌면서 이름만 관행으로 남았다. HTTPS의 S가 바로 이 TLS를 가리킨다.

## 자물쇠가 알려주지 않는 것

여기서 흔한 오해가 갈린다. HTTPS는 통신 구간이 도청당하지 않는다는 걸 보장하지, 그 사이트를 운영하는 주체가 믿을 만하다는 걸 보장하지 않는다. 피싱 사이트를 만드는 쪽도 손쉽게 인증서를 발급받아 자물쇠를 달 수 있다. 오히려 요즘은 HTTPS가 워낙 흔해져서, 자물쇠가 없는 사이트를 찾는 게 더 어렵다. 자물쇠 유무로 신뢰를 판단하던 시절의 감각이 지금은 잘 안 맞는다.

인증서 종류에 따라 검증 수준이 다르기도 하다. 도메인 소유 여부만 확인하는 가장 기본적인 인증서도 있고, 사업자 실체까지 확인하는 더 까다로운 인증서도 있다. 브라우저 화면에서는 둘 다 똑같은 자물쇠로 보이는 경우가 많아서, 이 차이를 눈으로 구분하기는 쉽지 않다.

## 그래도 자물쇠는 봐야 한다

로그인이나 결제처럼 민감한 정보를 입력하는 페이지라면 HTTPS 여부는 최소한의 확인 사항이다. 없다면 그 구간은 누구든 들여다볼 수 있다는 뜻이니, 그런 페이지에 개인정보를 넣는 건 피하는 게 맞다. 다만 그 이상으로, 도메인 주소가 정확한지, 링크를 어디서 받았는지까지 같이 봐야 한다. 자물쇠는 필요조건이지 충분조건이 아니다.

검색 결과 노출에서도 HTTPS가 유리하게 작용한다고 알려져 있어서, 요즘 새로 만드는 사이트치고 HTTPS를 안 쓰는 경우는 거의 없다. 그래서 자물쇠의 존재 자체는 더 이상 특별한 신호가 아니게 됐다. 특별한 건 오히려 그게 없는 쪽이다.

봉투가 봉인되어 있다고 해서 보낸 사람이 누구인지까지 알려주지는 않는다. 그 구분을 아는 것과 모르는 것 사이에, 클릭 한 번의 거리가 있다.

---
![대표 이미지](images/11_HTTP_vs_HTTPS/11_HTTP_vs_HTTPS_1_cover.png)

본문에 그림이 들어가면 좋을 자리는 아래와 같다. 실제 이미지는 아직 넣지 않았다.

〔이미지 자리 — 본문에서 1번째 논점을 설명하는 대목〕

〔이미지 자리 — 본문에서 2번째 논점을 설명하는 대목〕

〔이미지 자리 — 본문에서 3번째 논점을 설명하는 대목〕

〔이미지 자리 — 마지막 문단 바로 위〕

## 이미지 생성 프롬프트

1. A large padlock icon glowing confidently above a browser address bar, while a shadowy masked figure stands just behind the browser window unnoticed, suggesting the padlock signals encryption but not trustworthiness, flat vector illustration style, split-composition showing two contrasting concepts side by side, minimal color palette, no text in the image, 16:9 composition.
2. A split-composition illustration: on the left, an open postcard with visible handwritten text being read by a shadowy eavesdropper along a wire; on the right, a sealed envelope with a small padlock icon traveling safely along the same wire, flat vector illustration style, split-composition showing two contrasting concepts side by side, minimal color palette, no text in the image, 16:9 composition.
3. A browser address bar with a padlock icon shown twice: one padlock sitting above a friendly storefront, the other identical padlock sitting above a suspicious masked storefront, showing the same icon appearing on both trustworthy and untrustworthy sites, flat vector illustration style, split-composition showing two contrasting concepts side by side, minimal color palette, no text in the image, 4:3 composition.
4. Two certificate documents side by side, one thin and simple representing basic domain verification, the other thick with an official seal representing deeper identity verification, both displaying the same small padlock icon on top, flat vector illustration style, split-composition showing two contrasting concepts side by side, minimal color palette, no text in the image, 4:3 composition.
5. A person's hand hovering over a login form on a screen, checking both a padlock icon in the address bar and the address text itself with a magnifying glass, flat vector illustration style, split-composition showing two contrasting concepts side by side, minimal color palette, no text in the image, 4:3 composition.
