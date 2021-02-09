---
id: 58
title: blockquote Style 수정
date: 2005-04-19T13:01:49+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=58
permalink: /post/58
keywords:
  - CSS,코드
  - CSS,코드
  - CSS,코드
categories:
  - 워드프레스
  - 웹 디자인
---
나는 워드프레스에서 새글을 작성할 때 Blockquote(인용문)이라는 빠른태그를 자주 사용하는 편이다.

웹서핑을 하다보면, **blockquote**에 스타일쉿을 사용하여 예쁘게 꾸며논 블로그나 게시판을 쉽게 찾을 수 있다. 나 역시 박스 형식의 스타일쉿을 사용하곤 했는데, [Dmitri Von Klein의 블로그](http://www.dmitrivonklein.com/2004/06/fancy-pants-elitist)를 보고 따옴표로 바꿔봤다. 

> BLOCKQUOTE 요소는 인용한 단락을 표시할 때 사용합니다. BLOCKQUOTE는 Q 요소와는 달리 P나 TABLE과 같은 블록 요소를 포함할 수 있습니다. 하지만 BLOCKQUOTE 요소는 문단이나 인라인 요소 안에 포함될 수 없습니다. **출처 : Html 사전**

문제는 [LikeJazz님의 글](http://www.likejazz.com/29681.html)처럼 p 태그가 2개 이상 사용된 blockquote에서는 제대로 출력되지 않는다. 이는 출처 부분의 p 태그에 클래스를 하나 더 삽입해서 해결해야 한다.

사실, CSS2의 :after, :befere를 사용하면 이런 꽁수들을 모두 해결할 수 있다. 하지만, 인터넷익스플러가 이를 표현하지 못하기 때문에 일이 복잡하게 꼬이는 것이다.

<pre>blockquote {
background: url(/blog/wp-content/themes/Blix/images/spring_flavour/bq-bg-b.gif) no-repeat;
margin: 10px 10px;
padding: 5px 0 0 30px;
}
blockquote p {
background: url(/blog/wp-content/themes/Blix/images/spring_flavour/bq-bg-a.gif) no-repeat right bottom;
margin: 5px;
padding: 0 30px 5px 0;
}
</pre>

이 글의 스타일쉿은 [_여기_](/files/doc/2005-04/blockquote.css)에서 확인할 수 있다.