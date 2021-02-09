---
id: 45
title: Dynamic Korea 서브메뉴 때려잡기
date: 2005-04-14T22:44:43+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=45
permalink: /post/45
keywords:
  - dynamic-korea,CSS,work,코드
  - dynamic-korea,CSS,work,코드
  - dynamic-korea,CSS,work,코드
categories:
  - 웹 디자인
---
지난 [자랑스런 대한민국~](/blog/index.php/2005/04/08/37)이라는 글에서 밝혔듯이 Dynaimc Korea의 홍보활동을 위하여 30억의 예산을 사용했다고 한다. (그 돈의 1/10만 있어도 세상 편하게 살아갈 수 있을텐데&#8230; 쩝)

[<img src="/files/img/2005-04/d-k.gif" width="176" height="166" alt="다이나믹 코리아 서브메뉴" />](/files/doc/code/2005-04/dynamic-korea.html) 하지만 [Dynamic Korea 홈페이지](http://www.korea.net/)의 경우, 굳이 Html Validator를 사용하지 않고 **소스보기만 하더라도 복잡하게 뒤엉킨 table 태그들과 쓸데없이 남용되고 심지어 문법까지 틀린 Javascript 를 사용함을 알 수 있다.** 이는 웹페이지 로딩시간을 증가시키며, 웹브라우저-접근성 문제도 유발하고, 결론적으로 해외 네티즌들이 한국 웹사이트에 대한 좋지 못한 인상을 받을 것이다. 

Dynaimc Korea 홈페이지의 잘못된 태그와 Javascript 사용의 대표적인 예라고 할 수 있는 좌측에 위치한 서브메뉴를 올바른 코딩방법인 ul, li 코드와 스타일쉿에 의하여 나름대로 단순하게 구현해봤다. [완성된 페이지는 여기](/files/doc/code/2005-04/dynamic-korea.html)에서 볼 수 있다. (메뉴항목들은 hooney.net을 참고함 ^^;)

**사용된 CSS :** 

<pre>body {font: 12px/180% sans-serif; color:#505050;}
h3 {font: bold 14px/180% sans-serif; color: #3F8F98; margin: 0 10px}
.side1{width: 170px; margin: 10px; padding: 5px; background: #E4F6F4;}
ul, ul li, li ul, li ul li {margin: 0; padding: 0; list-style: none;}
ul li{padding: 5px 0;	display: block;}
li ul{border-top: 1px solid #BDDDD9;}
li ul li a{
	display: block;
	padding-left:25px; margin:1px 0;
	border-bottom: 1px solid #BDDDD9;
	color:#505050; text-decoration: none;
	background:url(bullet-1.gif) no-repeat 10px center;
}
li ul li a:hover {color:#246F44; background:#CFECE9 url(bullet-1-on.gif) no-repeat 10px center;}
* html li ul li a {height: 1%; /*IE야 언제 정신 차릴래?*/}
</pre>

스타일쉿을 확인하면 알 수 있겠지만, 계층형 구조는 스타일 코드를 단순화하는데 무척 편리하다.