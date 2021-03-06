---
id: 339
title: 웹 페이지 확대 보기와 마이티 마우스의 재발견
date: 2006-12-20T01:00:57+09:00
author: Hooney
layout: post
guid: http://hooney.net/2006/12/20/339/
permalink: /post/339
keywords:
  - 확대보기 기능,윈도우 비스타,22인치 와이드 모니터,마이티 마우스,엘라스틱 레이아웃
categories:
  - 웹 디자인
  - 추천/리뷰
---
최근 Internnet Explorer 7(IE7) 정식 버전이 출시되면서, 탭 브라우징, RSS 구독, 사용자 지정 검색창 등 다양한 기능들을 MS IE를 주로 사용하고 있는 국내 웹 사용자들도 활용할 수 있게 됐다.

<img src="/uploads/2006/ie7zoom.png" class="left" alt="인터넷 익스플러 7의 화면 확대 기능" title="인터넷 익스플러 7의 화면 확대 기능" height="239" width="201" /> 그 중에서 나는 기존 파이어폭스에서 제공하고 있지 않던 기능인 IE7의 화면 확대 기능이 무척 맘에 든다. 기존의 웹 페이지 확대 기능은 &#8220;%&#8221;나 &#8220;em&#8221;과 같은 상대적인 단위에 의존한 텍스트 크기 기반 확대였지만, Opera 9에서 화면 비율 확대 기능을 처음 선보인 이후, 이번에 IE7도 지원한 기능이다.

기존의 텍스트 크기 기반 화면 확대 기능의 경우, &#8220;px&#8221; 기반의 레스터 이미지(또는 배경이미지)를 확대할 수 없었기에 웹 디자이너가 의도한 웹 페이지의 스타일이 뒤틀려 보일 수 밖에 없었다. 물론 해외의 고급 웹 디자이너 경우, &#8220;%&#8221;나 &#8220;em&#8221; 같은 상대적 단위를 절묘하게 사용하여 텍스트 크기를 확대했을 떄도 디자인이 덜 깨질 수 있도록 다양한 기법(Elastic Layout)을 선보이기도 했다.

하지만 이와 같은 기법들은 무척 고도의 상대적 디자인 기법이기에, 디자이너와 사용자 모두에게 불만을 제공할 수 밖에 없었다. 대신에 Opera 9와 IE 7의 화면 비율 확대 기능은 화면을 디자인하기도 쉽고, 사용자도 보다 원활한 페이지 서핑이 가능하기에 디자이너와 사용자 모두를 충족시키는 완벽한 기능이라고 할 수 있다.

<img src="/uploads/2006/opera9zoom.png" alt="오페라 9 화면 확대 기능" title="오페라 9 화면 확대 기능" height="309" width="395" /> 

다가오는 2007년 가정용PC의 기본 사양은 22인치 와이드 LCD 모니터가 될 것이다. 내년 초에 출시될 윈도우 vista의 기본 기능인 사이드바를 효과적으로 활용하기 위해서, 마이크로소프트사는 22인치 와이드 모니터를 비스타의 추천 하드웨어로 권장하고 있다. 이에 많은(특히 델) 하드웨어 제작사들이 22인치 와이드 모니터를 주력 상품으로 준비하고 있다.

이렇게 크고 특히 가로로 긴 모니터를 사용하다보면, 현재의 웹사이트들이 기본적으로 채택한 1024&#215;768 해상도에서 전체창으로 볼 때를 가정하여 디자인된 레이아웃이 무척 답답하고 조악스럽게 느껴진다. 1680 이상의 가로 해상도를 지원하는 22인치 와이드 모니터에서 현재의 웹사이트를 전체창으로 볼 수 없다. 적당하게 브라우저 크기를 조절해서 보는 게 일반적일 것이다.

<img src="/uploads/2006/vista.png" alt="윈도우 비스타" title="윈도우 비스타" height="102" width="356" /> 

정해진(현재까지의 1025&#215;768) 브라우저 크기에 따른 레이아웃이 아닌, 사용자가 선택한 브라우저 크기에 유동적으로 대응할 수 있는 그런 웹 디자인이 필요할 것이다. 기존의 레스터 이미지 기반의 포토샵 중심의 웹 디자인에서 사용자 환경에 능동적으로 대응할 수 있는 CSS 디자인이 더더욱 중요해질 것이다.

최근 개편된 [gucci](http://www.gucci.com/us/us-english/us/fall-winter-06/unicef/) 웹 사이트를 보자. 이 사이트가 보여주는 가로 스크롤바가 웹 서핑에 불편을 주는가? 엊그제만 해도 가로 스크롤 바를 만드는 웹 사이트 레이아웃을 사용자 경험성에 의거하여 최악의 사용성 예제 사이트로 뽑곤했다. 하지만 와이드 모니터에 화면 확대 기능을 적절히 사용하게 된다면, 가로 스크롤바는 세로 스크롤 바보다 오히려 편리하게 다가올 수 있다.

<img src="/uploads/2006/index360scroll220050802.gif" class="right" alt="마이티 마우스의 4방향 스크롤" title="마이티 마우스의 4방향 스크롤" height="220" width="190" /> 다만, 가로 스크롤을 효과적으로 다룰 수 있는 방법이 제공되야 한다. 웹 브라우저가 포토샵처럼 기능키(예 ctrl) + 마우스 움직임이 화면을 잡고 이리저리 끌어 옮길 수 있는 기능을 제공하지 않는 현실에서, 가로 스크롤을 제공하는 마우스가 필요할 것이다.

이처럼 가로 스크롤을 제공하는 마우스는 애플의 마이티 마우스가 있다. 나처럼 저시력자가 야간에 웹 서핑을 하기 위해선 화면 확대 기능이 반드시 필요하며, 이 때 효과적으로 네비게이션할 수 있는 마이티 마우스가 필요하다.

마이티 마우스 하나 사놓구선, 자랑 글 한번 길게 쓴다. ㅎㅎ

추가) 파이어폭스에도 [화면 확대보기 기능을 지원하는 플러그인](http://update.mozilla.or.kr/addons/?p=763)이 개발됐습니다.