---
id: 64
title: CSS shorthand properties (단축 속성)
date: 2005-04-22T23:37:28+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=64
permalink: /post/64
keywords:
  - CSS,코드
  - CSS,코드
  - CSS,코드
categories:
  - CSS
---
[Rated-R님의 글](http://www.5pix.com/weblog/archives/000212.php)에도 소개된 것처럼, CSS 사용할때 단축 속성을 사용하면 코드를 줄일 수 있다.

이러한 CSS의 모든 속성에 shorthand properties(단축 속성)을 사용할 수 있는 것이 아닌, 아래의 몇몇 속성에서만 사용 가능하다.

  1. **font 단축 속성**  
    구문 : { font: font-style | font-variant | font-weight | font-size | line-height | font-family }  
    예제 : { font: 0.75em/1.4em 돋음, san-serif; }
  2. **margin 단축 속성**  
    구문 : { margin: margin-top | margin-right | margin-bottom | margin-left }  
    예제 : { margin: 1em 2em 3em 4em; }
  3. **padding 단축 속성**  
    구문 : { padding: padding-top | padding-right | padding-bottom | padding-left }  
    예제 : { padding: 1em 2em 3em 4em; }
  4. **border 단축 속성**  
    구문 : { border: border-width | border-style | color }  
    예제 : { border: 1px dotted #123456; }
  5. **border-top, border-right, border-botoom, border-left 단축 속성**  
    구문 : { border-top: border-width | border-style | color }  
    예제 : { border-top: 1px dotted #123456; }
  6. **list-style 단축 속성**  
    구문 : { list-style: list-style-type | list-style-position | list-style-image }  
    예제 : { list-style: url(&#8220;hooney.gif&#8221;) inside disc; }
  7. **background 단축 속성**  
    구문 : { background: background-color | background-image | background-repeat | background-attachment | background-position }  
    예제 : {background: #123456 url(&#8220;hooney.net&#8221;) no-repeat center left; }

위의 단축속성의 구문은 순서가 바껴도 IE6, FF1, NN7 등 대부분의 최근 브라우저에서 자동으로 해석해 주지만, 구식 브라우저(NN4, IE5 등)의 경우 바르게 표현하지 않는 문제가 있으므로, 가급적 단축속성 구문을 지켜야 한다.  
단, margin과 padding의 CSS 단축속성의 구문은 반드시 지켜져야 한다. (위에서부터 시계방향으로&#8230;)

톱 스타일(top style)과 같은 CSS 전문 프로그램에서는 자동으로 단축속성을 정리해주는 기능이 포함되어 있다.