---
id: 21
title: 워드프레스 DashBoard(알림판) Hack
date: 2005-04-04T17:08:56+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=21
permalink: /post/21
categories:
  - 워드프레스
  - 추천/리뷰
---
워드프레스를 사용하고 있는 많은 블로거들이 **DashBoard(알림판)에 대해 불만**을 토로한다. 워드프레스 개발자 블로그와 몇몇 관계 블로그의 글들을 RSS 로 긁어오는데 시간이 많이 걸리기 때문이다.

국내 어떤 블로거님은 워드프레스의 로그인에 소요되는 시간을 다른 설치형 블로그 툴과 비교하여 워드프레스를 깍아내리기도 했다.  
_(링크를 준비하지 못함. 네이버 블로그였음)_ 

>워드프레스 사이트에 들어가보면, 이런 DashBoard(알림판)을 혐오하는 나머지 다른 블로그 툴로 옮기는 사건까지 발생하는 것을 알 수 있다. 

> **[ 워드 프레스 Support 포럼에 올라온 글1 ]**  
> I got tired of the fat, resource-hogging DashBoard shipped with WordPress 1.5. It gets feed from God-knows-how-many WordPress blogs for no good reason and without my (or your) consent.  
> It comes up the first thing when you login to admin. I don&#8217;t like any of that. This thing downloads even when I am on my home setup running WordPress from localhost!

> **[ 워드 프레스 Support 포럼에 올라온 글2 ]**  
> Of course, that&#8217;s not the only problem with the Dashboard &#8212; it also takes a substantial time to load, even on fast servers with fast connections, simply because it&#8217;s dependent on other sources being available for syndication. When a DNS server was slow the other day, it took 72 seconds for the Dashboard to load here &#8212; admittedly, that&#8217;s the fault of the DNS server, but it proves the point nicely.

나 역시 이런 문제 때문에 DashBoard(알림판)을 삭제하고, 기본적인 카운터나 붙여서 사용할까 고민했었다. 마침 워드프레스 서포트 포럼에서 **DashLite 1.0, an alternative &#8220;Dashboard&#8221; for WordPress 1.5**를 발견하고 바로 설치해보았다.  
결과는 상당히 만족스럽다. 체감 로딩속도가 10배는 빨라진 것 같다. (체감속도임 ^-^) 더군다나 알림판도 더욱 효율적이다. 정말 워드프레스 사용자에게 절대 강추 Hack이다.

[<img src="/files/img/2005-04/_dashboard-hack.png" width="440" height="362" alt="대쉬보드 Hack - 미리보기" />](/files/img/2005-04/dashboard-hack.png)

Hack 파일은 [이곳](http://www.joahua.com/blog/wp-content/2005/03/wp-admin-index.txt)에서 다운받을 수 있다.  
다운받은 파일은 index.php로 이름을 바꿔준다.  
자신의블로그주소/wp-admin/에 복사(덮어쓰기)해주면 된다.  
혹시나 모를 문제에 대해서 기존의 index.php 파일은 백업해 논다.

스크린샷은 [이곳](http://www.joahua.com/blog/wp-content/2005/03/dashlite-full.jpg)에서 확인할 수 있다.  
제작자의 홈페이지는 http://www.joahua.com/blog/ 이다.

결코, 후회하지 않을 선택이라 확신한다.  
소스 몇몇 부분을 한글화하여 내가 사용중인 파일은 [이곳](/blog/wp-content/files/index.txt)에서 다운받을 수 있다. 

_한글 워드프레스를 사용할 때 발생했던 알림판(DashBoard)의 공식개발블로그의 RSS 날짜 문제는 곰님이 수정한 [한글 언어팩](http://heygom.com/wp-locale/ko_KR.tar.gz)을 적용하면 해결된다._