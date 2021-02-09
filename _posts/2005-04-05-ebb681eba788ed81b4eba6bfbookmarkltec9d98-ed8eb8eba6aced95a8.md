---
id: 23
title: 북마클릿(Bookmarklt)의 편리함
date: 2005-04-05T10:13:13+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=23
permalink: /post/23
keywords:
  - Bookmarklt
  - 북마클릿
  - 북마클릿
categories:
  - 워드프레스
  - 추천/리뷰
---
[GatorLog님의 글](http://gatorlog.com/blog/?p=8)을 통해서 워드프레스의 북마클릿이라는 유용한 기능을 알게 됐다.

> 웹을 항해하다가 어떤 웹페이지에 담긴 내용을 가지고 블로그 글을 쓰려고 한다면 이 툴바에 있는 북마클릿을 누르기만 하면 됩니다. 누름과 동시에 워드프레스 편집기가 팝업창으로 열리면서 제목과 웹페이지 링크가 자동으로 따라붙습니다. 이걸 이용해 링크블로그를 만든다면 그보다 더 편리할 수가 없을 것 같군요.

혹시나 해서 구글을 이용하여 검색해보니 상당히 많은 북마클릿이 존재하는 것을 알게 됐다. [위키페디아](http://en.wikipedia.org/wiki/Bookmarklet)에 의하면, 북마클릿의 의미는 쉽게 알 수 있다. 

> A bookmarklet is a small JavaScript program that can be stored as a URL within a bookmark in most popular web browsers, or within hyperlinks on a web page. Because Microsoft Internet Explorer uses the term favorites instead of bookmarks, bookmarklets are also less commonly called favlets or favelets.

이런 북마클릿의 선구자라고 불리우는 [Jesse Ruderman](http://www.squarefree.com/bookmarklets/)의 사이트에 보면 꽤나 유용한 것들을 발견할 수 있다. 그중에 나는 [Enlarge Textareas]((function(){var i,x; for(i=0;x=document.getElementsByTagName("textarea")[i];++i) x.rows += 5; })()) 와 [Zoom Images in]((function(){ function zoomImage(image, amt) { if(image.initialHeight == null) { /* avoid cumulating integer-rounding error */ image.initialHeight=image.height; image.initialWidth=image.width; image.scalingFactor=1; } image.scalingFactor*=amt; image.width=image.scalingFactor*image.initialWidth; image.height=image.scalingFactor*image.initialHeight; } var i,L=document.images.length; for (i=0;i<L;++i) zoomImage(document.images[i], 2); if (!L) alert("This page contains no images."); })();) 을 내 북마크바로 옮겼다.

이 2개의 북마클릿은 다음과 같은 유용한 기능을 제공한다.  
**Enlarge Textareas** &#8211; 글쓰는 공간을 늘여줌. 블로그에 글을 쓸 때 유용함. 특히 2줄 정도밖에 이용할 수 없는 답글을 길게 쓸때 유용하다.  
**Zoom Images in** &#8211; 이미지를 크게 보여준다.