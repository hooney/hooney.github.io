---
id: 304
title: 웹 접근성과 웹 저작
date: 2006-07-29T02:13:43+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=304
permalink: /post/304
keywords:
  - 웹 접근성,web authoring
categories:
  - 웹 접근성
---
웹 저작(Web Authoring)은 자주 사용되지 않는 단어였다. 1990년대 중반까지만 해도 웹 저작이라는 책도 출간됐지만, 실제 2000년대에 들어와선 그 단어적 의미가 퇴색된 게 사실이다.

하지만, 2000년대 들어 웹의 흐름을 바꾼 블로그가 탄생하면서 웹 저작의 중요성이 강조되고 있다. 웹 저작이라는 단어가 낯설다면, 블로그에 글을 쓰는 것이라고 생각하면 쉽게 이해할 수 있을 것이다.

웹 저작 도구로는 드림위버와 같은 이지윅 에디터 툴이나 에디트플러스 같은 텍스트 에디터 툴 외에도 블로그나 게시판에 글을 쓸때 이용하는 [FCKeditor](http://www.fckeditor.net/demo/default.html) 같은 이지윅 에디터도 포함한다.

[테터툴](http://www.tattertools.com/ko/)이나 [워드프레스](http://wordpress.org/)와 같은 GPL 기반 무료 블로그 툴도 이지윅 에디터를 포함하고 있는데, 이 에디터 툴이 잘못된 마크업을 생성하는 경우가 많다. 즉, 사용자(웹 저자)의 의도를 전혀 고려하지 않고, 전혀 구조적이지 못한 컨텐츠를 생성하는 것이다. 대표적인 예로, 문단을 p로 구분하는 게 아니라 br + br로 구분하거나, h1~h6과 같은 문서 제목을 사용할 수 없음은 물론이며, ul + ol과 같은 목록 대신에 ▶과 같은 전혀 의미없는 컨텐츠를 만들어 낸다.

일단 이런 웹 저작 툴에 대해서는 W3C 산하 [WAI](http://www.w3.org/WAI/intro/atag.php)는 물론이며, [국내 번역문 1)](http://gregshin.pe.kr/atag10/) [한국형 지침서 2)](http://www.iabf.or.kr/standard/View.asp?seq=31&gotopage=1&gotoblock=&find1=&find2=)에서도 충분히 언급하고 권고하고 있지만, 중요한 건 개발자들이 웹 표준을 제대로 인식하지 못하고 있는 점이다. 머리가 멍청하면 손발이 고생이라는 옛말처럼, 개발자가 제대로 된 에디터 툴을 만들지 않아서 사용자들이 자신의 의도와 전혀 상관없는 컨텐츠들을 만들고 있는 실정이다.

나는 워드프레스에서 이지웍 에디터를 사용하지 않고, 위키 문법으로 컨텐츠를 작성하며, 이를 서버측에서 다시 적절히 HTML 마크업으로 변환해서 컨텐츠를 생성하고 있다. 실제 HTML 마크업보단 위키 문법이 작성할 때 편리하며 유용하다. 위키 문법을 블로그나 게시판 등에 사용하고 싶다면, 간단한 플러그인을 추가하면 될 것이다.

최근 몇몇 사용자 분들이 내 블로그의 글들을 영어나 일본어로 번역해서 읽고 계신다. 몇일 전에 [HII 관련 글](/2006/07/347/)을 썼는데, 이 글은 여러 종류의 번역기를 이용해서 읽었다. 좋은 글도 별로 없고, 국내 사용자도 별로 없는 블로그에 외국인 사용자들이 방문해주셔서 황송할 따름이다. ^^;

나도 필요한 정보를 얻기 위해 해외 사이트를 자주 방문하는 편이며, 영어로된 문서는 사전([Fast dic](http://update.mozilla.or.kr/addons/?p=195))을 이용하고, 일본어로 된 문서는 번역기를 이용하는 편이다. 종종 웹에서 이렇게 외국어로 된 문서를 읽다보면, 사전이나 번역기로 해석할 수 없는 단어(방언, 속언 등)와 엉터리 문법으로 작성된 정보들로 인해서 정보에 접근하는 데 어려움을 겪곤 한다.

아무리 올바른 HTML 마크업으로 잘 구조화된 웹 문서라고 할지라도, 그 컨텐츠 자체가 구조적이지 않는다면, 정보에 접근하는데 어려움을 겪을 수 밖에 없다. HTML 마크업이 구조화되지 않은 것이 웹 개발자 때문이라면, 컨텐츠(정보)가 구조화되지 않은 것은 웹 저자의 무성의 때문이다.

핸드폰과 같은 소형 디스플레이 장치를 위해 컨텐츠를 요약문 형식으로 별도 제작한다면&#8230; 완전 멋진 저자라는 칭송을 받을 지도 모른다. ㅎㅎ

웹 사이트의 접근성을 향상시키는 것은 무척 많은 것들을 신경 써야만 가능한 일이다. HTML 마크업은 물론이며, 디자인도 신경 써야하며, 심지어 컨텐츠의 단어 하나, 문단 하나에도 신경써야 한다. 이렇게 만들어진 접근성이 향상된 웹 사이트는 검색엔진이든, 장애인이든, 다양한 웹 접속 도구를 통해서 정보에 접근하려는 사용자에게 그 가치를 인정받을 것이다. 그리고 나도 인정할 것이다. ^^;