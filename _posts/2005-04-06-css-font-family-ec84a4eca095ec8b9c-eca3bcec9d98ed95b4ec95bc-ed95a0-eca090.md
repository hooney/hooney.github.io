---
id: 32
title: 'CSS : font-family 설정시 주의해야 할 점.'
date: 2005-04-06T17:08:30+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=32
permalink: /post/32
keywords:
  - CSS,font
  - CSS,font
  - CSS,font
categories:
  - 웹 디자인
---
한국 모질라 사이트에서 [웹 표준화 프로젝트 포럼](http://forums.mozilla.or.kr/viewforum.php?f=9)에 가면, 정말 많은 것을 배울 수 있다. 국내에 웹 사이트들이 웹 표준을 지키고 OS나 브라우저와 관계 없이 접근성을 향상 시키기 위한 사이트 버그 신고 및 문제 해결을 위한 포럼인데, 웹 표준과 관련된 질문의 답변도 해주고 있다. _(나도 CSS2의 after, before에 관해 질문하적이 있음)_ 

이곳에서 [웹개발자는 Cross Browsing 가이드 참고하세요](http://forums.mozilla.or.kr/viewtopic.php?t=572) 라는 글이 있는데, 한국 소프트웨어 진흥원의 의뢰로 차니님이 작업한 [Cross Browsing 가이드 웹버전](http://www.mozilla.or.kr/docs/web-developer/standard/)을 볼 수 있다. 이 글의 내용도 무척 유용하지만, 딸린 답글들도 좋은 내용이 많다. 그 중에서 얼마전 웹디자인 작업할 때 참고 했던 내용이 있다.

CSS 제작시 font-family: 돋음; 이라고 하면 안 되고, font-family: 돋음, Dotum, Baekmuk Dotum, Undotum, Apple Gothic, Latin font, sans-serif; 이라고 해야 한다.

그 이유에 대해서는 신정석님의 답글을 인용하면,

> 돋음과 Dotum을 같이 써야 하는 이유는 비한국어 Windows (최소한 9x/ME)에서는 MS IE조차도 &#8216;돋음&#8217;을 인식하지 못 하기 때문입니다. Apple Gothic은 Mac OS X에 들어 있는 sans-serif에 해당하는 한국어 글꼴 이름입니다. 표 4에서 라틴 글꼴을 비교한 표가 있는데, Windows Corefonts는 다른 OS에서도 사용할 수 있습니다.

라기 때문이다.

이런 좋은 정보가 썩히지 않고 많은 사람들에게 알려졌으면 좋겠다.