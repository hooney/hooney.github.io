---
id: 17
title: 드림위버에 Text 붙여넣기
date: 2005-04-03T14:38:43+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=17
permalink: /post/17
keywords:
  - 드림위버,tip
  - 드림위버,tip
  - 드림위버,tip
categories:
  - 블로그
  - 웹 디자인
---
드림위버로 웹페이지 작업을 하면, 몇몇 문제에 부딪히곤 한다. 그 중 하나는 **인코딩 문제**이고, 다른 하나는 **Text 붙여넣기** 이다. 

드림위버는 UTF-8을 기본인코딩으로 설정되어있다.  
때문에 charset=euc-kr 을 명시하지 않은 html 소스의 경우에는 한글이 모두 깨져보이게 된다. 이는 제로보드 소스를 수정하다보면 쉽게 알 수 있다. (한글 주석이 모두 깨져보임)

한글이나 워드, 메모장 등 다른 프로그램에서 작성된 Text 내용을 드림위버로 가져올 때는 반드시 Text 붙여넣기로 해야 한다. 그렇지 않을 경우에는 다른 프로그램에서 미리 만들어 논 태그(눈에 보이지 않지만)들을 그대로 가져오게 된다.

이 부분은 한글(워드 프로그램)에서 작성한 내용을 Html 문서로 보내기를 해보면 쉽게 알 수 있다. 그냥 단순하게 만든 hwp 파일이 어마어마하게 많은(솔직히 불필요한) tag를 가진 html로 변환되는 것을 소스보기를 통해 자세히 알 수 있다.

이런 문제 때문에, 대부분의 드림위버 사용자들은 키보드 단축키 설정(일반적으로 **ctrl + shift + alt + V**)을 통해 Text 붙여넣기를 사용하고 있다.

![text copy](/files/img/2005-04/textcopy.gif) 

> 이 글은 블로그코리아에서 서핑중에 어느 블로거님의 글을 보고 트랙백 용으로 작성한 글이다. 난 생 처음 트랙백을 해본다.