---
id: 333
title: Virtual PC를 이용한 IE6, IE7 함께 사용하기
date: 2006-12-02T11:06:56+09:00
author: Hooney
layout: post
guid: 'http://hooney.net/2006/12/02/virtual-pc%eb%a5%bc-%ec%9d%b4%ec%9a%a9%ed%95%9c-ie6-ie7-%ed%95%a8%ea%bb%98-%ec%82%ac%ec%9a%a9%ed%95%98%ea%b8%b0/'
permalink: /post/333
categories:
  - 추천/리뷰
---
[현석님의 글](http://hyeonseok.com/soojung/browser/2006/12/02/309.html)에서 [Virtual PC를 이용한 IE6, IE7 함께 사용할 수 있다](http://blogs.msdn.com/ie/archive/2006/11/30/ie6-and-ie7-running-on-a-single-machine.aspx)기에 바로 설치해봤습니다. [MS가 제공하는 IE가 들어 있는 가상 이미지](http://go.microsoft.com/fwlink/?LinkId=70868)는 ie6을 구동하기 위해 최소화된 window xp professinal sp2를 OS로 사용하고 있습니다.

파일 다운로드에서 설치, 구동까지 너무 쉽게 되는 것 같더니만, 역시나 문제가 발생하더군요. 바로 한글이 제대로 출력되지 않는 문제가 있더군요. 혹시나 해서 IE 설정에서 글꼴을 확인해보니, 영문을 제외하고는 한글/일본어 글꼴/중국어 글꼴 등 비영어권에서 사용하는 글꼴이 설치되어 있지 않더군요.

<img src="/uploads/2006/ie6vm.jpg" alt="Virtual PC를 이용한 IE6" height="400" width="500" /> 

Virtual PC를 첨으로 사용하는지라, 구글신의 도움으로 여러 방법들을 시도했지만 결국 좌절입니다. 아무래도 Virtual PC용 이미지 파일에 한글 폰트를 추가하는 건 쉽지 않아보입니다. MS도 이 VPC 이미지 파일을 2007년 4월 1일부로 파기시킨다니, MS에 한글 폰트(굴림/돋움/바탕/궁서체)를 추가해 달라고 요청하기도 어려울 것 같습니다.

이로써 한글 폰트의 중요성을 다시 한번 깨닫게 됐지만, 결과적으로는 토요일 오전을 쓸 데 없는 짓을 하느라 허비한 것 같네요. 이제 슬슬 아침먹고 24시 2부나 봐야 할듯&#8230;

(추가) 한글 폰트를 설치하는 과정을 포함하여, VPC를 통해 IE6를 설치하는 과정 전반을 [Nosyu님 글](http://nosyu.egloos.com/2826468)에서 확인하실 수 있습니다.