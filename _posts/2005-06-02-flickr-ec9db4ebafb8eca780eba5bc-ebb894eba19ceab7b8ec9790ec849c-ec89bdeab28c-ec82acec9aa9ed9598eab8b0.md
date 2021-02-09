---
id: 108
title: Flickr 이미지를 블로그에서 쉽게 사용하기
date: 2005-06-02T11:21:52+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=108
permalink: /post/108
keywords:
  - flickr,hack,블로그,코드
  - flickr,hack,블로그,코드
  - flickr,hack,블로그,코드
categories:
  - 블로그
  - 추천/리뷰
---
플릭커는 매력중에 하나는 이미지들을 쉽게 RSS로 긁어 올 수 있는 점이다. [Flickr 홈페이지](http://www.flickr.com/)에서 클릭 몇번으로 간단하게 이미지들을 긁어올 수 있는 방법을 제공하고 있다. 테터툴이나 워드프레스와 같은 설치형 블로그툴 뿐만 아니라 홈페이지도 사용 가능하다. 국내에도 이와 유사한 서비스가 있으면 얼마나 좋을까? ㅜ.ㅜ

플릭커에서 제공해주는 방법은 복잡한 테이블 레이아웃으로 이미지를 긁어오기 때문에, 그동안 나는 [WP Flickr-RSS 플러그인](/blog/index.php/2005/05/27/117)을 사용했었다. 하지만 이 또한 역시 불러오는 방법이 1개로 제약되는 문제가 있었다. 다른 플러그인을 찾다가 결국은 Flickr에서 제공해주는 코드를 직접 수정해 보았다. 

http://Hooney.net 첫화면의 우측에서 Flickr 이미지를 긁어올 때 사용한 html :

<pre><h2>
  Flickr images
</h2>


<div>
  
</div>
</pre>

나는 이미지를 보여주는 우측부분의 특성 때문에 h2와 div를 사용했다. 이들은 굳이 사용할 필요가 없다. Flickr 자바스크립트의 간단한 규칙을 이용하면, 이미지들을 다양한 방법으로 긁어올 수 있다.

* `id=11338328@N00` &#8211; 사용자 ID 지정  
* `count=6` &#8211; 긁을 이미지 개수 지정  
* `display=random` &#8211; 긁을 방법 지정  
* `size=square` &#8211; 긁을 이미지 크기(thumbnail,medium,square) 지정  
* `raw=1` &#8211; 플릭커 링크 안보이기(보이려면 raw=0) 지정

자바스크립트로 긁어온 이미지들을 좀 더 예쁘게 다듬기 위해서 적절히 CSS를 사용했다.

http://Hooney.net 첫화면의 우측에서 Flickr 이미지를 긁어올 때 사용한 CSS :

<pre>span.flickr {
	color:#FF0084;
	} /* Flickr의 분홍색(r) */
div.flickr {
	margin:0 10px 15px 10px
	} /* 박스 여백때문에 사용 */
.flickr img{
	width:55px;
	height:55px;
	margin:3px;
	} /* 이미지 크기지정(원래:75px) */
.flickr a img{
	border:1px solid #aaa;
	padding:2px;
	} /* 이미지 외곽선 색 + 여백 */
.flickr a:hover img{
	border-color:#FF0084;
	} /* 마우스를 올렸을떄, 이미지 외곽선의 분홍색 */
</pre>

Jsvascript와 CSS를 응용하면, 블로그 글에 여러 이미지들을 앨범식으로 나타낼 수 있을 것이다. 플릭커 이미지를 불러오는 다양한 예제는 다음 글에 설명해보련다. ^^;;

앗. 이 방법의 최대 문제는 자바스크립트에 &, = 의 사용으로 인해서 html-valiiation을 통과하지 못한다는 것이다. 이 녀석을 사용하기 전까지만 해도 xhtml-stric valiation을 통과했었는데, 이제는 바로 불합격이다. 다른 방법을 생각해봐야 하는가.. ㅠ.ㅠ