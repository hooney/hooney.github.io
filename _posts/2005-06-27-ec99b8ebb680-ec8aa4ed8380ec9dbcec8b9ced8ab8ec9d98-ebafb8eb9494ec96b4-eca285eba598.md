---
id: 146
title: 외부 스타일시트의 미디어 종류
date: 2005-06-27T15:55:21+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=146
permalink: /post/146
categories:
  - CSS
  - 웹 접근성
---
So-Basic 테마의 CSS는 공개용의 경우 screen과 print용 2종류의 미디어 형식으로 배포되고 있지만, 내가 사용하고 있는 것은 오직 screen용 하나뿐이다. 솔직히 프린트용 외에는 별도의 CSS의 필요성을 느끼지 못했던 나였지만, TJpak님께서 [Hooney.net 블로그를 PDA에서 테스트한 글](http://www.tjpark.com/web2/board/view.php?db=us&cn=11)을 보고 인식이 많이 바뀌게 됐다. 특히 [Eric Meyer의 Cascading Style Sheets, 2nd Edition](/archives/2005/06/26/current-reading-css-book/)라는 책을 보면서 외부 스타일시트의 미디어 종류와 역할 등을 자세히 알게됐다.

#### 외부 스타일시트를 웹문서에 연결할 때 사용하는 코드 :

``

#### 외부 스타일시트의 미디어 종류 :

all
:   모든 미디어 속성에 사용. 별도로 지정하지 않으면 기본값으로 사용.

aural
:   발음 장치, 스크린 리더기, 그 외의 다른 오디오 문서 해석 장치에 사용

braille
:   점자용 화면에 사용

embossed
:   점자용 프린트에 사용

handheld
:   핸드폰이나 PDA와 같은 휴대용 디지털 기기에 사용

print
:   프린트하거나 프린트 미리보기에 사용

projection
:   프로젝터에 사용

screen
:   웹브라우저에 사용

tty
:   고정폭 문자열을 가지는 장치용 (텔레타이프, 터미널, 저사양의 휴대용 기기 등). tty 미디어 타입의 경우 픽셀 단위를 사용하면 안됩니다.

tv
:   TV에 사용

#### 외부 스타일시트의 미디어 종류를 다수로 설정 :

``

또한 Alternate 스타일시트를 사용하면 별도의 자바스크립트를 사용하지 않고도 스타일시트를 교체해서 사용할 수 있다. FF, Mozila, Opera처럼 최근에 나온 웹브라우저는 Alternate 스타일시트를 지원하고 있다. 사용자들이 이런부분에 익숙해진다면, 별도의 자바스크립트를 사용하는 일이 적어질 것이다. 먼저 IE6에서 벗어나야만 이런 기능을 느낄 수 있을 것이다.

#### Alternate 스타일시트 사용 :

`` //큰글씨로 보여주는 CSS  
``> //작은글씨로 보여주는 CSS

Alternate 스타일시트 사용예 : ([일몰님 블로그](http://ilmol.com/))  
<img src="/files/img/2006-06/ilmol-css.png" width="395" height="241" alt="일몰님 블로그" /> 

개인적으로 글씨 크기를 제어하는 CSS를 별도로 제작하는 것보다는 브라우저에서 ctrl + 마우스휠을 위아래로 이동시키거나, 모질라 계열 브라우저에서 ctrl + +, &#8211; 키를 누르는 것을 알려주는 편이 더 좋을 것 같다. 굳이 별도의 CSS를 제작한다면 낮/밤의 시간별이나 계절별, 또는 날씨별로 제작하는 것이 효율적일 것 같다.