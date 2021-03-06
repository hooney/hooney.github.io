---
id: 354
title: CSS 구문과 선택자
date: 2007-02-06T08:11:34+09:00
author: Hooney
layout: post
guid: http://hooney.net/2007/02/06/354/
permalink: /post/354
categories:
  - CSS
  - 웹 디자인
---
dojo 자바스크립트 툴킷이 [dojo.query](http://blog.dojotoolkit.org/2007/02/04/dojoquery-a-css-query-engine-for-dojo)라는 dojo를 위한 CSS Query Engine을 공개했다. CSS Query Engine이란 HTML DOM structures를 CSS 선택자로 접근할 수 있도록 하여, 보다 쉽고 빠르며 효율적으로 DOM을 이용할 수 있는 방법을 제공한다.

이 CSS Query Engine라는 단어는 [IE7 스크립트 라이브러리](http://dean.edwards.name/IE7/notes/)를 개발한 Dean Edwards가 2004년에 처음 사용한 것으로 알고 있다. 그는 이미 [cssQuery](http://dean.edwards.name/my/cssQuery/)를 개발해서 배포중이다. 또한 [jQuery](http://jquery.com/), [MochiKit](http://mochikit.com/), [Prototype](http://www.prototypejs.org/), [behavior.js](http://bennolan.com/behaviour/)들도 CSS 선택자 형식으로 DOM에 접근할 수 있는 CSS Query Engine이다.

CSS는 아래의 그림처럼 선택자와 선언으로 구성되며, 선언은 속성과 값으로 구성된다.  
<img src="/uploads/2007/cssSeltor.png" alt="css 선택자" title="css 선택자" height="212" width="296" /> 

2년 전, [현석](http://hyeonseok.com/)님은 CSS에서 선택자의 중요성을 아래처럼 한마디로 표현했다.

> 선택자를 알면, CSS의 절반을 안다.

위의 그림에서 볼 수 있듯이, CSS의 문법상 선택자는 CSS의 절반이다. 그렇다고, 단순히 문법상에서 선언(속성+값)과 동등한 위치에서 선택자가 절반의 위상을 갖는 것으로 오해하면 안된다. CSS의 핵심인 속성의 상속(inherit)과 겹침(cascade)을 효과적으로 사용하기 위해선 CSS 선택자를 명확히 이해해야하기 때문에 그 비중이 CSS의 다른 모든 것들을 합친 것과 동등한 비중을 갖는다는 뜻이다.

CSS를 얼마나 잘 사용하느냐는 것은 CSS 선택자를 얼마나 잘 사용하느냐와 같다. CSS를 처음 작성하는 초급 CSS 디자이너나 왠만큼 작성해봤다는 중급 CSS 디자이너의 CSS를 비교해 보자. 둘 코드의 차이를 한눈에 파악할 수 있을 것이다. 즉, 고급 CSS 디자이너는 CSS 선택자를 효율적으로 사용하여, 디자인 시안을 단순히 코드로 옮기는 것이 아니라, 눈에 보이지 않는 디자인 영역까지 촘촘히 디자인하는 것이다. (말로 표현하기엔 아직 나의 내공부족인듯.. ㅠ.ㅠ)

CSS 선택자를 잘 사용하기 위해선, 나무를 보지 말고 산을 봐야만 한다. 즉, [뫼 산 CSS 디자인 프로세스](/2006/04/17/263/)를 익힐 필요가 있다.