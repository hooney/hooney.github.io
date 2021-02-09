---
id: 173
title: CSS로 유연한 디자인 만들기
date: 2005-07-27T13:08:46+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=173
permalink: /post/173
keywords:
  - em,CSS,font-size
  - em,CSS,font-size
  - em,CSS,font-size
categories:
  - CSS
  - 웹 디자인
---
우리는 옛부터 전해지는 타이포그래피의 금언에서부터 시작해야 할 것이다. 단락에서 가장 읽기 좋은 라인의 길이는 &#8216;알파벳 한 세타 길이의 하나 반&#8217;이다. 이것은 최대의 가독성을 위해서 문단의 각 라인은 약 문자 40개 정도의 길이가 되어야 함을 의미한다.

이것이 어떻게 유동적 페이지라는 우리의 목표와 상응될 수 있을까? 만일 우리가 화면을 가득 채우도록 디자인된 페이지를 만든다면 라인 길이를 제어할 수 없으며, 그렇게 되면 가독성 같은 것은 포기해야만 할 것이다.

하지만 두 가지 모두 가질 수는 없을까? 가능하다.

먼저 우리는 고정된 폰트 크기에 대한 관념을 포기하는 것부터 시작해야 한다. CSS는 우리에게 타이포그래피에 대한 폭 넚은 제어권을 주고 있다. 또한 그것은 몇 가지 새로운 측정 단위들을 주는데, 가장 주목할만한 것은 em 단위이다.

포인트나 픽셀이 절대적인 크기를 나타내는 것과는 달리, em은 폰트에 기반하고 있다. 기술적으로 1em은 당신이 어떤 폰트를 사용하든 소문자 &#8216;m&#8217;의 폭을 나타내도록 되어 있다. 

대부분 브라우저들은 이렇게 복잡하지는 않지만 실제로 1em을 &#8216;기본값&#8217;으로 정의하고 있다. 그래서 인터넷 익스플러4(영문 기준) 혹은 그 이상의 버전에서 1em으로 정해진 베르다나체(verdana)는 12pt로 렌더링된다.

그러나 그것은 고정적인 12pt가 이니고, 오히려 사용자가 임의로 정한 기본값이라고 할 수 있다. 만일 시력이 약한 사용자(나 포함)가 브라우저에서(환경설정 메뉴를 사용하여) 폰트 사이즈를 16pt까지 키워서 기본값으로 설정한다면 1em은 16pt가 되는 것이며, 모든 것이 이것에 맞추어 크기가 조정될 것이다.

당신은 대부분의 사용자들이 결코 그들의 환경설정을 바꾸지 않는다고 말할 것이다. 그 말은 맞다. 나(hooney)는 밤늦게 일을 마치고 새벽에 해외 사이트의 작은 글꼴의 영문으로된 웹문서들을 읽어야 했을떄, pt나 px 크기를 절대값으로 고정시킨 웹디자이너들을 무척 저주했다. 나의 지친 눈에 그런 웹문서들의 양이 얼마나 많은지.. 쩝.

&#8211; 출처 : 웹디자인 마인드 &#8211;