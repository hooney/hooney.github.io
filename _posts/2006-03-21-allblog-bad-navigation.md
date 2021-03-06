---
id: 251
title: 올블로그의 플래시 네비게이션
date: 2006-03-21T09:47:17+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=251
permalink: /post/251
keywords:
  - 올블로그,플래시,네비게이션
categories:
  - 블로그
  - 워드프레스
  - 웹 접근성
---
오전에 방문한 [올블로그](http://www.allblog.net/Home/)가 예전과 미묘한 차이점이 있는 것을 발견하고, 확인해보니 상단 네비게이션이 사라졌다. 흡사 구글과 같은 느낌이었는데, 어떤 이유 때문인지 올블로그 개발자가 잠시 네비게이션을 숨겨놓은 줄 알았다.

[<img src="/uploads/thumb_allblog-2.png" width="450" height="136" alt="올블로그 메인 페이지" />](/uploads/allblog-2.png)

나의 상상력에 개연성이 부족한 것 같아서 다시 확인해보니, 사용중인 파이어폭스 브라우저의 웹디벨로퍼 툴바에서 자바스크립트가 꺼져 있는 것을 알 수 있었다.

파이어폭스 사용자들이 가장 많이 다운받는 플러그인 중 하나가 [NO-Scipt](https://addons.mozilla.org/extensions/moreinfo.php?application=firefox&numpg=25&id=722&page=comments&pageid=4)일 정도로, 최근 웹사이트들의 극심한 자바스크립트 사용에 불만을 갖는 사람들이 많다. 나 역시도 Ajax로 도배된 사이트를 방문할 땐 자바스크립트를 끄는 편이다.

_이때문에 플래시 네비게이션이 제대로 작동하지 않는 것은 단순히 사용자들의 잘못이 아니라 개발자들의 잘못이다._

  * 플래시를 사용하여 네비게이션을 제작한 문제 &#8211; [object 태그 안](http://hyeonseok.com/pmwiki/index.php/Markup/Object)에서 ul, li 등으로 별도의 네비게이션을 제공할 수 있다.
  * 자바스크립트를 네비게이션에 사용한 문제 &#8211; [nopscript를 이용](http://trio.co.kr/webrefer/html40/interact/scripts.html#h-18.3)하여 ul, li 등으로 별도의 네비게이션을 제공할 수 있다.

결국, IE의 설계 변경에 따른 플래시 네비게이션을 자바스크립트 꽁수로 대처하는 방법에 문제가 있음을 알 수 있다. noscript 태그의 사용법과 대체 네비게이션 제공이라는 웹 접근성의 기본을 명시하지 않은 점이다.

우리가 명심해야 할 것은 장애인만이 웹 접근성의 수혜자는 아니라는 사실이다.