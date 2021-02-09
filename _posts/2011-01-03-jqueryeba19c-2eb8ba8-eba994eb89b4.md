---
id: 768
title: jQuery로 2단 메뉴 구현, 따라하기
date: 2011-01-03T21:27:58+09:00
author: Hooney
layout: post
guid: http://hooney.net/?p=768
permalink: /post/768
categories:
  - 코드
  - 후니넷
---
&#8220;jQuery&#8221;나 &#8220;jQuery 탭&#8221;, &#8220;jQuery 메뉴&#8221; 검색어로 후니넷에 방문하는 분들이 많은데, [무려 4년 전인 2007년에 작성한 글](/2007/08/20/431/)만 보고 되돌아가기에, jQuery로 가로형 2단 메뉴를 구현하는 코드를 업데이트합니다.

위키백과에선 아래와 같이 jQuery를 소개합니다.

> jQuery는 [자바스크립트](http://ko.wikipedia.org/wiki/%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8)와 [HTML](http://ko.wikipedia.org/wiki/HTML "HTML") 사이의 상호작용을 강조하는 경량화된 [웹 애플리케이션 프레임워크](http://ko.wikipedia.org/wiki/%EC%9B%B9_%EC%95%A0%ED%94%8C%EB%A6%AC%EC%BC%80%EC%9D%B4%EC%85%98_%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8C%ED%81%AC)이다. 존 레식에 의해, [2006년](http://ko.wikipedia.org/wiki/2006%EB%85%84 "2006년") 뉴욕 시 [바캠프](http://ko.wikipedia.org/wiki/%EB%B0%94%EC%BA%A0%ED%94%84 "바캠프")(Barcamp NYC)에서 릴리즈되었다.
> 
> jQuery는 [MIT 라이선스](http://ko.wikipedia.org/wiki/MIT_%EB%9D%BC%EC%9D%B4%EC%84%A0%EC%8A%A4 "MIT 라이선스")와 [GNU 일반 공중 사용 허가서](http://ko.wikipedia.org/wiki/GNU_%EC%9D%BC%EB%B0%98_%EA%B3%B5%EC%A4%91_%EC%82%AC%EC%9A%A9_%ED%97%88%EA%B0%80%EC%84%9C "GNU 일반 공중 사용 허가서")의 [듀얼 라이선스](http://ko.wikipedia.org/w/index.php?title=%EB%93%80%EC%96%BC_%EB%9D%BC%EC%9D%B4%EC%84%A0%EC%8A%A4&action=edit&redlink=1 "듀얼 라이선스 (존재하지 않는 문서)") 하의 [자유 오픈 소프트웨어](http://ko.wikipedia.org/w/index.php?title=%EC%9E%90%EC%9C%A0_%EC%98%A4%ED%94%88_%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4&action=edit&redlink=1 "자유 오픈 소프트웨어 (존재하지 않는 문서)")이다.

[jQuery API 문서](http://api.jquery.com/)를 참고하지 않더라도, 국내에 jQuery에 대한 책도 많이 출간됐고 많은 분들이 블로그나 카페에 관련 팁을 공유해주셔서, 쉽게 jQuery를 익힐 수 있습니다. 이 글이 아직 jQuery를 어려워하는 웹 디자이너나 처음 웹 사이트를 만드는 분들에게 도움이 됐으면 합니다. [완성된 2단 메뉴(GNB)를 먼저 확인해주세요.](/files/test/jqueryNav.html)

![jQuery로 2단 메뉴 따라하기](/wp-content/uploads/2011/01/jqueryNavigation.gif) 

본론으로 바로 들어가서, **HTML 코드**를 작성합니다.

<div class="oembed-gist">
  <noscript>
    View the code on <a href="https://gist.github.com/hooney/9c0e0148af21c4f352a4213e288044b7">Gist</a>.
  </noscript>
</div>

다음으로, 스타일을 부여하기 위해 **CSS 코드**를 추가합니다.

<div class="oembed-gist">
  <noscript>
    View the code on <a href="https://gist.github.com/hooney/9c0e0148af21c4f352a4213e288044b7">Gist</a>.
  </noscript>
</div>

마지막으로, 2단 메뉴로 동작하기 위해 **JavaScript(jQuery) 코드**를 추가합니다.

<div class="oembed-gist">
  <noscript>
    View the code on <a href="https://gist.github.com/hooney/9c0e0148af21c4f352a4213e288044b7">Gist</a>.
  </noscript>
</div>

$(&#8216;#nav li&#8217;).bind(&#8216;mouseenter keyup&#8217;, function() { // 메뉴바의 각 메뉴들에 마우스를 올리거나 키보드로 이동하면,  
$(this).addClass(&#8216;on&#8217;).siblings().removeClass(); // 해당 메뉴에 클래스 on을 추가하고, 다른 메뉴의 클래스를 제거합니다.  
}); // 네. 3줄로 끝입니다.  
  


[완성된 2단 메뉴(GNB)를 확인](/files/test/jqueryNav.html)해주세요. 이 코드는 IE8, [IE Tester](http://www.my-debugbar.com/wiki/IETester/HomePage)를 이용한 IE7, [windows XP mode](http://windows.microsoft.com/ko-KR/windows7/install-and-use-windows-xp-mode-in-windows-7)를 이용한 IE6, Firefox 3.6, Chrome 9에서 테스트했습니다.

jQuery의 매력에 빠져보실 분에겐 [실전 jQuery 쿡북(요리책)](http://www.aladin.co.kr/shop/wproduct.aspx?ISBN=8996276553)을 추천합니다. 비싼만큼, 도움이 될 것입니다. 🙂