---
id: 208
title: 민트 사용시 인코딩 변경
date: 2005-09-16T15:48:36+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=208
permalink: /post/208
keywords:
  - encording
  - encording
  - encording
categories:
  - 블로그
  - 워드프레스
---
웹사이트 방문자 통계(카운터) 프로그램인 [민트](http://www.haveamint.com/)를 사용하다보면, 한글 검색어 부분이 깨지는 것을 확인할 수 있다. 페이지 뷰나 리퍼러 체크를 할때는 한글이 깨지지 않지만, 검색어 목록 중에서만 한글이 깨지는 것을 알 수 있다.

<img src="/files/img/2005-09/mint-1.png" width="345" height="184" alt="민트의 검색어 스크린샷" /> 

이는 민트의 문자 인코딩이 iso-8859-1로 설정되어 있는 문제 때문이다. iso-8859-1 역시 국제 표준화된 문자 인코딩이지만, 아쉽게도 한국어(korean)를 지원하지 않기 때문에 UTF-8로 바꿔줘야 한다.

워드프레스와 태그(tag, keyword)를 알기 전에는 검색어를 통한 사이트 접근에 대해서 전혀 개념이 없었지만, 구글의 키워드 검색 시장이 사라지지 않는 한 검색어는 사이트 운영에 무척 중요한 자료가 될 것이다.

민트의 문자 인코딩을 수정하는 방법은 http://민트설치폴더/app/display.php 에서 content=&#8221;text/html; charset=iso-8859-1&#8243; 부분을 utf-8로 수정해주면 된다.

물론 요상망측(인코딩 설정이 없는)한 검색사이트를 통해서 접근한 검색어의 경우에는 제대로 확인할 수 없다. 국내 사이트들이 작은 한국에서만 발버둥치지 않길 바랄 뿐이다. 🙂