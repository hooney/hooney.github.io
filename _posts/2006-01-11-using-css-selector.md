---
id: 235
title: CSS 선택자 남용 유감
date: 2006-01-11T11:23:23+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=235
permalink: /post/235
categories:
  - 웹 디자인
  - 웹 접근성
---
[CSS](http://www.w3.org/Style/CSS/)는 Cascading Style Sheet의 약자이다. 의역하면, 계단형(상속형) 스타일 시트이다. CSS는 (x)Html의 외양을 꾸미는 역할을 하며, 이름에서 알 수 있듯이 CSS의 가장 큰 특징은 상속형이다. 각각의 CSS 요소들의 정의된 성질들이 조상/자손, 부모/자식 관계 속에서 상속된다는 것이다.

이렇게 상속되는 특징을 잘 이해하고, CSS를 제작한다면, 웹문서는 출렁이는 파도처럼 부드러움을 갖게될 것이다. 웹사이트 전체적인 통일성과 유동성을 쉽게 구성할 수 있고, 추후 수정/보완할 수 있다.

그렇지 않고 CSS를 제작한다면 흡사, 웹문소의 구성요소들은 각개전투를 벌이다가 웹사이트 전체적인 전투진형을 흩뜨릴 것이며, 장군(제작자)의 작전명령을 오만년이 걸려서야 수행할 것이다. ^^;

이런 상속되는 특징을 이해하기 위해선 먼저 [CSS 선택자](http://trio.co.kr/webrefer/css2/selector.html)를 이해해야 한다. 즉, CSS 선택자 이해 -> CSS 상속성 이해 -> CSS 이해가 되려남.. 이와 관련해서 [현석님](http://www.hyeonseok.com/)은 &#8220;선택자를 알면 CSS의 절반을 안다&#8221;라고 말했었다.

최근 UTF-8 인코딩을 지원하고, 웹표준을 준수한 [GR보드가 공개됐다.](http://sirini.net/grboard/board.php?id=grskin&articleNo=29) 또한 개인화기능이 추가되고, 웹표준을 준수한 [올블로그V2](http://v2.allblog.net/)가 베타 테스트 중이다. 이 두 사이트가 웹표준을 준수한다고 해서 코드를 잠깐 확인해보니, CSS 선택자(Html 요소, Class 선택자, ID 선택자)가 남용된 걸 알 수 있었다.

웹 유효성 검사(Validate)는 수단이지 목적이 아니다. 검사를 통과했다고 표준도 아닐 것이다. 충분히 의미있고(sementic), 구조적인(Structual)인 마크업을 사용하도록 조금 더 노력한다면, 정말 멋진 사이트가 될 것이다.

GR보드와 올블로그 개발자 여러분 조금 더 힘내세요! 파이팅~!