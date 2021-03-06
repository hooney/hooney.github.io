---
id: 330
title: NHN UI Library 오픈? 유출?
date: 2006-11-17T16:59:58+09:00
author: Hooney
layout: post
guid: 'http://hooney.net/2006/11/17/nhn-ui-library-%ec%98%a4%ed%94%88-%ec%9c%a0%ec%b6%9c/'
permalink: /post/330
keywords:
  - NHN,네이버,UI,Library
categories:
  - 추천/리뷰
---
네이버와 한게임을 운영하고 있는 [NHN의 UI Library](http://html.nhndesign.com/)가 오픈됐다. 이미 해외에선 [Yahoo! User Interface Library(YUI)](http://developer.yahoo.com/yui/)가 작년에 오픈되어 전세계 UI 개발자들과 다양한 의사소통을 해오고 있었지만, 국내에선 UI 관련 정보를 공유하는 사이트를 NHN이 처음으로 오픈했다.

[<img src="/uploads/2006/naver-ui-library.gif" alt="NHN UI Library" height="330" width="500" />](http://html.nhndesign.com/)

NHN의 UI Library는 얼마전 다음에서 공개한 API와 서버측 개발자들의 공간인 [DNA](http://dna.daum.net/)를 겨냥한 것으로 볼 수 있는데, 서버 사이드와 클라이언트 사이드 개발이라는 엄연한 차이가 있기 때문에 서로 선의의 경쟁을 할 수 있을 것 같다.

&#8220;Naver와 Hangame 서비스 웹페이지 UI 개발시 참고할 내용을 담고 있는 이 사이트&#8221;에 UI 개발 관련 다양한 정보와 사내 UI 개발팀에서 운영하는 블로그로 이뤄져 있으며, 다음의 DNA와 함께 국내 웹 개발 관련 자료의 공유에 많은 도움이 될 것이다

다만, NHN UI개발팀에서 말하는 &#8216;HTML 개발시 주안점&#8217;에 시멘틱(sementic)이 빠져서 아쉽다. html은 문서의 구조를 위한 마크업이고, 의미를 부여하기 위한 마크업이기 때문이다.

[<img src="/uploads/2006/coding_nhn2.gif" alt="nhn coding 주안점" height="274" width="500" />](http://html.nhndesign.com/blog/?p=10)

예를 들어, 문서의 어느 한 문맥을 강조하기 위해서 CSS를 통한 스타일 가이드로써 녹색을 지정했다고 하자. 그렇다면 이 문맥을 표현하기 위해서 html에선 class=&#8221;green&#8221;을 사용해야 할까? 아니다. 만약 그렇게 사용했다면, font color=&#8221;green&#8221;과 다름없는 형식(presentation)을 위한 마크업을 한 것과 다름 없다.

[<img src="/uploads/2006/naver-html-name.gif" alt="nhn html 네이밍" height="243" width="486" />](http://html.nhndesign.com/guide_css.html)

정답은 em을 사용하고, CSS에서 em {color:green}을 사용해야 한다. 웹 문서의 어느 한 문맥을 강조하는 것이 html의 역할이지, green이라고 class/id 네이밍을 통한 시각적 마크업을 사용하는 것은 올바르지 않다.

구조와 형식, 그리고 동작의 명확한 분리가 이뤄졌을 때에 비로서 웹은 보다 정보가 충만한 시멘틱 웹이 될 수 있을 것이다.