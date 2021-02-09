---
id: 52
title: align=”center”의 올바른 표현
date: 2005-04-17T21:43:55+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=52
permalink: /post/52
keywords:
  - CSS,tip
  - CSS,tip
  - CSS,tip
categories:
  - 웹 디자인
---
테이블을 기반으로 웹페이지의 레이아웃을 할때, 글이나 이미지 등의 내용을 가로방향으로 가운데 정렬을 하기 위해서는 align=&#8221;center&#8221; 태그를 사용한다. 하지만, 지난 글에서 밝힌 것과 같이 _테이블 태그은 자료의 정리와 표현을 위한 태그이지 결코 레이아웃을 위한 태그가 아니다._ 

xhtml + css 에는 align=center 가 없다. 대신 스타일쉿에서 **margin : 0 auto;** 를 이용한다. 이는 margin : 0 auto 0 auto; 의 단축코드로써 마진값(바깥여백)을 위에서부터 시계방향으로 위=0, 오른쪽=자동, 아래=0, 왼쪽=자동을 준다는 의미이다. 

인터넷 익스플러 6과 파이어폭스 1에서는 위와 같은 방법으로 가운데 정렬을 할 수 있지만, **인터넷 익스플러 5.5 이하 버전에서는 text-align : center 핵(hack)을 사용**해야 한다.

내 컴퓨터에는 IE 6, FF 1, NN 7이 깔려 있기 때문에 css 기반 디자인을 할 때 test-align : center 핵을 깜빡 잊고 코딩에서 빼먹기도 한다. ^_^