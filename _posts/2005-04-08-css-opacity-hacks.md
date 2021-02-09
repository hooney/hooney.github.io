---
id: 35
title: CSS opacity Hacks
date: 2005-04-08T10:09:34+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=35
permalink: /post/35
categories:
  - 웹 디자인
---
[<img class="left" src="https://i2.wp.com/files/img/2005-04/zoto3.jpg?resize=155%2C312&#038;ssl=1" alt="전남대" height="312" width="155" data-recalc-dims="1" />](/files/doc/2005-04/opacity.html)

웹디자인 작업시 보통 롤오버 이미지를 만들 때는 Adobe Imageready나 Macromedia Fireworks를 이용한곤 한다. 특히 Fireworks는 드림위버와 연동되는 코드와 자바스크립트를 자동으로 생산해주기 때문에 롤오버 메뉴 버튼 등을 만들때 자주 이용했었다.

그러나 이런 프로그램들의 대부분이 Table-Layout으로 태그를 생산하기 때문에, Xthaml-css 에서 권장하는 div, ul, ol, li 태그들로 변경하기 위해서는 또 다시 Hand-Coding을 요구했다.

이런 문제들은 CSS : alpha 필터를 이용하면, 쉽게 해결할 수 있다. **우측의 이미지를 클릭** 해보자. 별도의 자바스크립트를 요구하지 않으며, 롤오버 이미지도 필요 없다. 결과적으로 CSS 코딩의 특징인 코드가 무척 단순해지며, 이에 따라 코드의 수정 및 재생산도 편해진다.

이 페이지의 [예제는 이곳](/files/doc/2005-04/opacity.html)에서 확인할 수 있으며, 사용된 [CSS는 이곳](/files/doc/2005-04/opacity.css)에서 확인할 수 있다.

**CSS opacity은 CSS3에서 지원하는 속성으로 CSS2에서는 지원하지 않는다.** 다만 인터넷익스플러, 파이어폭스, 사파리 등 최근 버전의 브라우저에서 자체적으로 지원하고 있는 CSS 속성일 뿐이다. 그러므로 현재지원되고 있는 W3C의 CSS Validator를 통과할 수 없다. [CSS3 opacity 속성에 대한 설명은 W3C에서 확인할 수 있다.](http://www.w3.org/TR/2003/CR-css3-color-20030514/#opacity)

_아.. code 퀵태그가 잘 안먹는다. 이거 먼가 대책이 필요한데&#8230; 코드 안에_ 

 _가 나오면 어떡하냐?!! 결국 txt 파일 다운로드로 대처해야 하는가!_