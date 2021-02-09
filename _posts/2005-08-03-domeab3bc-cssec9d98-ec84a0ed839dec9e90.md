---
id: 187
title: DOM과 CSS의 선택자
date: 2005-08-03T12:24:24+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=187
permalink: /post/187
keywords:
  - dom. javascript,CSS
  - dom. javascript,CSS
  - dom. javascript,CSS
categories:
  - CSS
---
몇일째 JS와 DOM과 관련된 책을 읽고 있다. 아무래도 남은 휴가기간은 내일과 모래에는 다른 일을 해야할 것 같기에, 일일 풀타임 독서도 오늘로써 끝일 것 같다.

JS와 DOM에 관련된 국내 서적을 찾기는 생각보다 쉽지 않다. 대부분은 활용팁들의 예제를 중심으로 설명된 책들이라 기본 원리에 대한 깊숙한 접근(마치 수학 정석 교제에서 공식을 증명하는 단계와 같은)을 하고 싶던 나로써는 W3C 사이트로 발길을 돌릴 수 밖에 없다.

[DOM(문서 객체 모델)](http://www.w3.org/TR/DOM-Level-2-HTML/)에 접근할수록, [CSS2의 selector(선택자)](http://www.w3.org/TR/CSS21/selector.html)가 자꾸 떠오른다. CSS의 선택자는 인터넷 익스플러가 거의 지원하지 않는 요소이기에, 국내 CSS 활동가들은 물론이고 해외 CSS 활동가 사이에서도 거의 논의 대상에서 빠져 있는 것 같다.

CSS의 선택자를 통해서도 어느정도(완벽할 순 없고) 문서 객체 모델에 접근할 수 있을 것이다. JS와 DOM을 이용해서 각 개체의 스타일 속성을 변경하는 것보다는 CSS로 접근하는 편이 훨씬 편하고 쉽다고 생각한다. (문제는 역시 IE의 미비한 지원이겠지만..)

현재로써 CSS의 선택자에 대한 정보를 얻을 수 있는 거의 유일한 방법은 W3C에서 권고된 [CSS 문서](http://www.w3.org/TR/CSS21/selector.html) 뿐인 것 같다. (혹시 관련 정보를 다루고 있는 국내 서적이나 국내 사이트를 아시는 분은 정보 좀 공유해 주시길..)

[CSS3의 선택자들](http://www.w3.org/TR/2001/CR-css3-selectors-20011113/#selectors)은 CSS2의 선택자들보다 그 양에서만 2배 가까이 늘어난 것 같다.