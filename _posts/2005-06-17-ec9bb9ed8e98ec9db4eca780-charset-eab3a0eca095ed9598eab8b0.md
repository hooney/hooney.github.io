---
id: 125
title: 웹페이지 Charset 고정하기
date: 2005-06-17T22:40:43+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=125
permalink: /post/125
keywords:
  - charset,utf-8,htaccess,mod_rewrite
  - charset,utf-8,htaccess,mod_rewrite
  - charset,utf-8,htaccess,mod_rewrite
categories:
  - 웹 디자인
---
제작중인 워드프레스 테마의 404 템플릿 페이지의 캐릭터셑(charset) 인코딩을 UTF-8로 지정해도 브라우저에서 EUC-kr로 읽는 문제가 있어서 지윤님과 msn으로 열심히 방법을 강구했다.

유니코드 전용 웹편집기로 새로 저장을 해봤지만 문제가 해결되지 않기에, 서버측의 http-config 문제인 것으로 판단하고 방법을 찾아보니 .htaccess 파일에 `php_value default_charset "utf-8"`의 한줄만 추가하면 쉽게 해결할 수 있었다.

다음에라도 같은 문제가 발생하면, 쉽게 해결할 수 있을 것 같다. 단, 아파치 서버에서 mod_rewrite 기능을 지원하지 않으면 사용할 수 없는 방법이기에 다른 방법도 한번 찾아봐야 겠다.