---
id: 207
title: 드림위버 8의 환경 설정
date: 2005-09-15T22:18:12+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=207
permalink: /post/207
categories:
  - CSS
---
드림위버 8를 설치하여 사용중인 [제이님](http://www.getografik.com/)이 오후에 MSN으로 내게 물어왔다. 디자인 모드에서 폰트 크기를 em으로 설정하면, 제대로 랜더링 되지 않는다는 것이다.

이는 MX 2004 버전에도 발생했던 문제인데, 한글 프로그램의 경우 디자인 모드에서 기본 글꼴의 크기가 12pt로 설정돼 있는 반면, 영문 프로그램의 경우 글꼴의 크기가 10pt로 설정돼 있기 때문이다.

[웹표준화 프로젝트](http://www.webstandards.org/)에서는 웹 접근성 측면에서 스크린 미디어 타입에서는 글꼴의 크기의 단위를 em으로 설정하도록 권하고 있다. 물론, 구식 브라우저에서는 제대로 랜더링되지 못하는 문제가 발생하지만, 접근성이라는 웹의 근본 정신을 생각한다면 가급적 사용하도록 노력해야할 글꼴 단위이다.

아직까지 한글 버전의 드림위버 8이 출시되지도 않았고, 드림위버는 한글 버전보다 영문 버전이 오히려 익숙해지는 데 편하기 때문에, 프로그램 환경 설정을 변경할 필요가 있다.

## 드림위버 8 환경 설정(ctrl+U) 변경하기 : (그림 참조)

<img src="/files/img/2005-09/mm-dreamweaver8.png" alt="드림위버 환경설정 창" height="300" width="500" /> 

기본 설정값인 10pt(small)을 비례폭 글꼴과 고정폭 글꼴은 12pt(medium) 크기로 변경하고 코드뷰용 글꼴은 10pt(small)로 변경하면, 글자를 볼때 딱 좋을 것이다.

이 방법을 알려줄 때 쯤, 이미 제이님은 혼자서 해결해버렸다. ([멋쟁이 제이님](http://www.getografik.com/))