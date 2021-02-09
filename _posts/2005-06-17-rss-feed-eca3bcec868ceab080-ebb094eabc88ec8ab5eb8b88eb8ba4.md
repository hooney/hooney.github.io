---
id: 122
title: RSS feed 주소가 바꼈습니다.
date: 2005-06-17T13:38:55+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=122
permalink: /post/122
keywords:
  - 새소식,fermalink,rss
  - 새소식,fermalink,rss
  - 새소식,fermalink,rss
categories:
  - 후니넷
---
**지난 2주 정도의 공백기간을 지나면서, Hooney.net의 퍼멀링크(permalink)가 대폭 수정되었습니다.** 기존의 /blog/index.php/feed/ 였던 RSS feed 주소가 </feed/>로 변경되었습니다.

리퍼러를 확인해보니, 예전 퍼멀링크로 글이나 RSS feed에 접근하는 경우가 무려 70%가 넘습니다. ㅜ.ㅜ 글을 예전 퍼멀링크로 접근할 경우 404에러 페이지가 뜨거나 인코딩이 깨져보입니다. 현재 Hooney.net은 전체 로딩 페이지 중에서 60% 이상이 404에러 페이지랍니다. RSS feed도 무슨 문제가 있는지 블로그라인외에는 긁어오는 구독기가 없습니다. 블로그라인의 경우에도 /blog/index.php/feed/의 예전 퍼멀링크로 접근할 경우, 글이 2개씩 보여지는 문제가 있네요.

겨우 20여명의 블로그라인 구독자가 있는 hooney.net에서 RSS feed 변경 공지를 띄우게 됩니다. 혹시 변경 사실을 모르고 계신 구독자분이 있다면, RSS feed 주소를 수정해주시면 고맙겠습니다. 🙂

lunamoth님이 가르쳐준 방법에 의하면, </blog/wp-rss2.php>을 이용하면 블로그라인 외의 다른 RSS 구독기에서도 정상적으로 구독할 수 있다고 하네요. 🙂

여러 종류의 RSS feed 리더기로 확인해본 결과, 워드프레스에서 제공하는 3 종류의 RSS0.95, RSS2, ATORM feed 중에서</feed/rss/>가 가장 잘 읽힙니다. 즉 가장 구식버전인 RSS2가 제대로 읽혀지네요. 이건 뭔가 문제가 있는듯 싶습니다. ^^;