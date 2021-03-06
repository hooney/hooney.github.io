---
id: 384
title: 변경된 구글 코리아의 첫 화면을 뜯어 보자.
date: 2007-05-30T16:40:24+09:00
author: Hooney
layout: post
guid: http://hooney.net/2007/05/30/384/
permalink: /post/384
categories:
  - CSS
  - 웹 디자인
  - 웹 접근성
  - 추천/리뷰
---
[구글 코리아](http://www.google.co.kr/)의 첫 화면이 변경됐다. 기존에는 로고에만 1개의 이미지를 제공할 정도의 텍스트 기반 페이지였는데(현재 [google.com](http://www.google.com/webhp?hl=en)처럼), 이번에 여러가지 아기자기한 아이콘이 추가됐다. 특히 검색 영역 아래쪽에 위치한 구글 서비스로 바로 갈 수 있는 링크들을 제공하는 점이 눈에 뛴다.

[![구글 한국](/wp-content/uploads/2007/05/google-kr.png)](/wp-content/uploads/2007/05/google-kr.png "구글 한국")

내 경우에는 구글을 검색 뿐만 아니라, GMail, Gtalk, Gcalendar, Gnote, Gdesktop, Ggroup 등 다양한 서비스 등을 이용하고 있기에 [Google My Account](https://www.google.com/accounts/ManageAccount)를 시작 페이지로 구정해서 사용해오고 있었다. 하지만, 이번에 구글 코리아의 첫 화면이 변경됐기에, 시작 페이지 주소를 변경해야겠다.

추가된 바로가기 링크에 마우스를 오버할 때, 아이콘이 변경되는 것을 확인할 수 있다. 플래시를 이용하면 쉽고 빠르게 표현할 수 있는 기법이지만, CSS와 JavaScript만으로 플래시 못지 않게 부드럽게 표현한 점이 놀랍다. 플래시가 설치되지 않은 브라우저, 또는 플래시를 사용할 수 없는 텍스트 브라우저에서도 해당 텍스트와 링크를 이용할 수 있도록 배려한 점이 맘에 든다.

### 구글 코리아의 서비스 바로가기 아이콘에 사용된 이미지 1개

[![구글 코리아에서 부가 서비스 바로가기 아이콘에 사용된 이미지](/wp-content/uploads/2007/05/svc_sprite_all.gif)](/wp-content/uploads/2007/05/svc_sprite_all.gif "구글 코리아에서 부가 서비스 바로가기 아이콘에 사용된 이미지")

1개의 배경이미지만으로 마우스가 오버될 때, Javascript로 CSS의 위치지정(position)을 바꿔주는 방법을 사용하여 부드러운 온오프 효과를 보여주고 있다. 정지된 GIF 이미지와 CSS + Javascript로도 플래시의 모션 그래픽 못지 않게 부드러운 효과를 나타낼 수 있는 것을 보여준 좋은 사례로 꼽을 수 있다. 다만, 키보드로 이동할 때를 고려하지 않은 점이 아쉽다. ㅎㅎ

이번 구글 코리아의 첫 화면 개편은 국내 웹 디자이너에게 많은 자기개발과 고민을 할 수 있는 동기를 부여했다. 시각 장애인과 같은 사람은 물론이고, 검색엔진과 같은 기계에게도 접근성 높은 사이트를 디자인하는 것이 결코 1990년대식의 초라한 웹 디자인으로 돌아가지 않아도 된다는 것을 보여줬기 때문이다.

### CSS와 Javascript를 이용한 다양한 네비게이션 효과 몇개

  * [CSS Dock Menu (Jquery + CSS)](http://www.ndesign-studio.com/demo/css-dock-menu/css-dock.html)
  * [Mini Slide Navigation](http://www.sgclark.com/sandbox/minislide/)
  * [Faster Page Loads With Image Concatenation (구글 코리아에서 사용하는 방법)](http://borkweb.com/story/faster-page-loads-with-image-concatenation)

꼬릿말1) 많은 사람들이 구글 코리아 첫 화면에 많은 이미지를 사용했다고 하는데, 시각적으로만 그럴뿐이며 실제는 3개만 사용됐다. &#8220;구글 로고, [검색 아이콘 세트](http://google.co.kr/ig/f/YkU7DYyz7v8/intl/ALL_kr/tab_sprite_all.gif), [서비스 아이콘 세트](http://www.google.co.kr/ig/f/AaEyQnOaAr4/intl/ALL_kr/svc_sprite_all.gif)&#8221; 이렇게 3개의 이미지를 CSS의 배경 위치 변경 기법을 이용하여 여러개 처럼 보이게 한 것이다.

꼬릿말2) 사용자들은 방문한 웹 사이트가 어떻게 만들어졌는지 전혀 고민하지 않는다. 하지만 웹 개발자와 디자이너는 수많은 고민과 노력을 통해서 보다 나은 웹 사이트를 만들어가고 있다. 로딩 속도를 0.00001초라도 빠르게 하기 위해서, 시각 장애인도 접근하고 이용할 수 있도록 하기 위해서, 최고의 웹 사이트를 만들기 위해서 노력하는 그들이 진정한 챔피언이다.