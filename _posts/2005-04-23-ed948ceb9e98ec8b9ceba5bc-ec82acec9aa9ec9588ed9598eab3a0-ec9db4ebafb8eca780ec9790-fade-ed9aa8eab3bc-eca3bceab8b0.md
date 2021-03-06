---
id: 65
title: 플래시를 사용안하고 이미지에 fade 효과 주기
date: 2005-04-23T10:38:24+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=65
permalink: /post/65
keywords:
  - effect,javascript,photo
  - effect,javascript,photo
  - effect,javascript,photo
categories:
  - 웹 디자인
  - 추천/리뷰
---
이미지를 플래시를 통해 보여주는 이유 중의 하나는 바로 Fade 효과이다. 플래시는 모션트윈 생성을 통해서 알파값만 조절해주면 간단하게 이미지 fade 효과를 나타낼 수 있다. 

http://www.couloir.org/ 에 가보면, **플래시를 사용하지 않고 메인이미지에 Fade 효과를 주고 있음**을 알 수 있다. 꽤 유용한 기술이라 생각해서 나름대로 검색엔진을 돌려보니 [Cagnut의 글 중에서 Onload image fades without Flash](http://clagnut.com/sandbox/imagefades/)를 발견할 수 있었다. 

CSS의 opcity 속성값을 비교적 단순한 자바스크립트를 사용을 통하여 이미지 fade 효과를 훌륭하게 표현하고 있다. 물론, W3C의 CSS, XHTML Validator를 통과하고 있다. 간단한 이미지 fade 효과는 플래시를 사용하는 것보다 이 기술을 사용하는 것이 더 효율적일 것 같다. 🙂