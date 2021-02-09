---
id: 112
title: 워드프레스 주소(URI) 변경하기
date: 2005-06-07T23:59:30+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=112
permalink: /post/112
categories:
  - 워드프레스
---
WordPress는 여러 파일들과 폴더들로 구성되어 있습니다. 대부분의 사용자들은 웹폴더를 효율적으로 관리하기 위해서 wordpress를 /blog/ 또는, / 로 설정합니다. 

/blog/ 보다는 /의 조금이라도 짧은 URI가 방문자들의 블로그에 대한 접근성을 높혀주기 때문에, php 및 js를 이용하거나, 또는 mod_rewrite를 이용해서 루트폴더에 있는 index 파일을 리다이렉트 시키곤 합니다. 

하지만, 이방법 역시 uri 주소를 리다이렉트시키는 것 뿐이지 퍼멀링크를 변경시키는 방법은 아닙니다. 이 문제를 해결할 수 있는 방법을 소개합니다. 출처 : [WordPress 공식 홈페이지의 지원포럼](http://wordpress.org/docs/installation/different-address/)

#### 아래처럼 블로그 주소를 옮긴다고 가정하면,

  * 워드프레스가 설치되어 있는 주소 -> /blog/
  * 워드프레스를 옮기려고 하는 주소 -> /

#### 4개의 해야할 일 :

  1. 워드프레스 관리자 페이지의 설정 > 일반에서 블로그 주소만 http://hooney.net으로 수정합니다. (단, 워드프레스 주소는 /blog 그대로 유지)
  2. 워드프레스 인덱스 파일인 /blog/의 index.php 파일을 root 폴더인 /으로 복사합니다.
  3. 복사한 인덱스 파일을 메모장으로 열어서 require(&#8216;./wp-blog-header.php&#8217;); 부분을 require(&#8216;./blog/wp-blog-header.php&#8217;); 로 수정합니다.
  4. .htaccess 파일을 이용해서 mod_rewrite 기능을 사용하고 있다면, 관리자 페이지의 설정 > 변하지 않는 링크에서 새로 고침 버튼을 클릭합니다.

끝났습니다. 너무 쉽게 변경되서 놀랍나요? 훗. 그게 바로 wordpress의 매력이랍니다. ㅎㅎ