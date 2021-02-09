---
id: 239
title: '웹사이트 개발과정 &#8211; 3'
date: 2006-01-12T17:05:17+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=239
permalink: /post/239
categories:
  - 웹 디자인
---
이제 div 태그를 삽입해서 레이아웃을 구성해보자. 미리 생각하고 있는 레이아웃이 있다면 상관없겠지만, 그렇지 않다면 [리틀 박스](http://www.thenoodleincident.com/tutorials/box_lesson/boxes.html)에서 맘에 드는 레이아웃을 골라보자.

[지난번에 작성한 html](http://csslook.com/file/doc/process-060112/2.html)은 [CSSLook.com](http://csslook.com)의 첫화면(홈페이지)를 구성할 것으로, 상단+몸통+하단 구성에 몸통은 소개+갤러리+뉴스의 3단 구성으로 레이아웃을 작성할 계획이다.

먼저 상단을 분리시키기 위해서, 드림위버에서 1번째 머릿글(로고)과 메뉴들을 마우스로 선택한다. 그리고 드림위버 상단 메뉴에서 삽입(alt+I) -> 레이아웃 객체(Y) -> Div 태그(D)에서 나오는 메시지 창의 ID 입력란에 header를 작성하면 된다. 

<img src="/files/img/2006-01/dw-4.png" width="500" height="284" alt="드림위버에서 Div 태그 삽입" /> 

_드림위버는 키보드 단축키를 변경해서 사용할 수 있는데, Html을 할때 자주 사용하는 Div 태그 삽입이나 순차/비순차 목록 삽입, 링크 삽입 등은 단축키를 지정해놓으면 편리하다._ 

이와 같은 식으로 몸통(body또는 contents)도 div로 나고, 하단 부분도 나눈다. 앗. 지난번 html 작성할 때, 하단 부분의 내용을 빠뜨렸는데, 이제 추가하면 된다. 보통 하단에는 카피라이트와 주인장 이메일 주소 등이 나오는데, 적당히 작성해보자.

지난 번에 하단 부분을 작성하지 않은 것을 실수라 생각할 수도 있겠지만, 일부러 빠뜨린 부분이다. 많은 사람들(특히 클라이언트)은 눈에 보이는 결과만을 중요시 여기겠지만, 이는 웹문서의 기본을 이해하지 못한 행위다. 인쇄된 문서는 다시 수정할 수 없지만, 웹문서는 언제든지 수정할 수 있는 특징이 있다. 어차피 구차한 변명인감.. -_-;

어쨓거나 위의 div 태그 삽입을 통해서 분리된 모습은 [예제3](http://csslook.com/file/doc/process-060112/3.html)과 같다. 결코 [예제2](http://csslook.com/file/doc/process-060112/2.html)와 다른 점이 없다고 분노하면 안된다. 아직 CSS를 통해서 몸양을 꾸미지 않았을 뿐이다. **지금까지 작업은 그림 그리기 위해서 팔레트를 구분시킨 것 뿐이며, 이제 CSS를 통해서 물감을 짜서 캔버스에 붓으로 그린다고 생각해보자~** 룰루랄라~