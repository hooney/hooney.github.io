---
id: 24
title: '파이어폭스의 워드프레스 북마클릿에 대한  버그'
date: 2005-04-05T11:11:50+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=24
permalink: /post/24
keywords:
  - bookmarklet,워드프레스,파어이폭스
  - 북마클릿,워드프레스,파어이폭스
  - 북마클릿,워드프레스,파어이폭스
categories:
  - 워드프레스
---
다른 블로거들은 어떨지 모르겠는데, 나의 경우엔 원도우2003의 환경에서 파이어폭스1.01를 이용하여 워드프레스를 북마클릿을 이용하다 보면, 새창이 메인창 뒤로 숨는 문제가 발생한다.

처음엔 파이어폭스의 탭브라우징 플러그인의 문제 인줄 알았는데, FastDic이나 QuickNote는 이런 문제를 발생하지 않기에 워드 프레스의 버그인 줄 알았다. 어차피 사용도 잘 안하는 북마클릿이니 그런문제가 있어도 별로 어려움을 겪지 않았다.

우연히 웹서핑 중에 알게 됐지만, http://ask.metafilter.com/mefi/12998 을 보면, 파이어폭스에서 워드프레스의 북마클릿의 새창이 뒤로 숨는 문제에 답변을 구하는 글을 확인할 수 있다. 이는 비단 워드페스 뿐만 아닌 MT에서도 발생하는 문제이다.

여러 답글이 있지만, 명확한 해답은 찾을 수 없다.  
좀 더 진지한 고민은 http://javascript.weblogsinc.com/entry/1234000217038812/ 에서 찾을 수 있는데, 1/10초 이하의 로딩시간을 갖는 팝업창에 대해서는 파이어폭스의 메인창 뒤로 숨겨지게 하는 것을 1초로 늘임으로써 해결하고 있다.

이에 관한 패치는 [버그질라](https://bugzilla.mozilla.org/show_bug.cgi?id=232605)에서 찾을 수 있다.

그럼에도 불구하고, 아직까지 나는 워드프레스 북마클릿을 거의 사용하지 않고 있다. 그 유용함은 충분히 알겠는데, 링크 블로그에 대한 의미조차 정확히 알지 못하기 때문이다.