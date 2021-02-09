---
id: 107
title: WordPress Short-State 플러그인
date: 2005-06-01T17:39:51+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=107
permalink: /post/107
keywords:
  - counter,블로그
  - counter,블로그
  - counter,블로그
categories:
  - 워드프레스
  - 추천/리뷰
---
몇일 전에 봤던 블로그툴 비교에 관한 글(bbc 출처의 pdf였는데, 원본을 못찾겠음 ㅜ.ㅜ)에서 WordPress를 깎아 내리는 내용 중에 하나가 바로 카운터 기능의 부재였다. 물론 카운터 기능이 블로그에 있어서 어느정도 필수적이긴 하겠지만, 반드시 있어야만 한다고 생각하지는 않는다. 나 역시 블로그에서 카운터(해외에선 state라는 단어를 일반적으로 사용함)를 사용하게 된 건 불과 몇일전이다. 

나는 예전에 [@hof님이 소개해준 BAstate](http://www.hof.pe.kr/archives/1103/)를 잠깐 사용하다가(WP 1.5.1 이후 버전에서는 사용불가), [한날님이 배포중인 한날카운터](http://www.hannal.com/blog/hannal_counter/)를 한동안 사용했었다. 음악바톤 관련글 이후 좀 더 다양한 기능을 지원하다가 [BlogCounter](http://blogcounter.de/)를 사용했었지만, 페이지 로딩속도가 현저하게 느려지는 것을 확인하고 다른 카운터를 찾게 됐다.

페이지 로딩속도를 위해서, 예전의 탈춤 일러스트도 제거하고, 기타 자잘한 이미들을 대부분 삭제했으며, 구글 애드센스도 제거했는데, 블로그카운터 때문에 느려지는 걸 보고만 있을 수 없었다. 그렇게 몇일을 보내다가 발견한 것이 바로 워드프레스 Short-State 플러그인이다.

[<img src="/files/img/2006-06/sstate.gif" width="282" height="147" alt="심플한 상태?" />](http://dev.wp-plugins.org/wiki/wp-shortstat)

[Jeff Minard](http://jrm.cc/)가 만든 플러그인으로 [이곳](http://dev.wp-plugins.org/wiki/wp-shortstat)에서 다운받을 수 있다. BlogCounter처럼 그래픽을 지원하진 않지만, RSS feed에 대한 카운터를 지원하는 점이 새롭다. http://shauninman.com/ 에서 좌측을 보면 shortstate를 쉽게 알수 있다. 특별히 RSS feed에 대해서 신경을 쓰지 않던 나였기에, 사이트를 방문하는 횟수보다 RSS를 수집해가는 횟수가 훨씬 많다는 사실이 충격이다. 하긴, RSS 수집기가 하루에도 수차례 방문하는 게 당연할 것이다. ^^;

이제 겨우 사용한지 3일째인데, 잡아먹은 DB가 그동안 블로그에 글을 쓰면서 사용한 DB의 2/3에 육박한다. 특별히 DB 사용에 제한이 없다면 무척 추천할만한 WP 전용 카운터다.

나는 이와 함께 서버에서 지원해주는 [AXS Visitor Tracking System](/axs/ax-admin.pl) 라는 오픈소스 카운터를 사용하고 있다. AXS Visitor의 경우 [WP의 플러그인을 이용하면 웹페이지에 있는 링크들의 클릭수를 분석해주는 기능](http://thedeadone.net/?p=184)도 있다. 이녀석은 오픈소스 카운터중에서 가장 최신 버전으로써, 너무 많은 기능을 지원하면서, 특히 온라인상에서 one-click 인스톨을 지원하고 있기 때문에 일반적인 웹사이트 카운터에 적절할 것 같다. 단 영어의 압박을 이겨내야 한다.

정말 많은 카운터 프로그램들이 있고, 각각 장단점이 있기 때문에, 자신의 계정 환경이나 필요한 기능에 따라 골라 사용하면 될 듯 싶다. 너무 많은 카운터는.. 왠지 모를 구속감을 줄 수도 있으니 적절한 수의 카운터를 사용함을 추천한다.

(이글은 [Camino님이 Blogcounter가 사라진 것을 지적](/blog/index.php/2005/05/31/125#comments-3)해줘서 쓰게 된 글임)