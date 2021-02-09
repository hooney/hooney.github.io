---
id: 712
title: Google Font API로 아름다운 웹 만들기
date: 2010-05-20T11:16:15+09:00
author: Hooney
layout: post
guid: http://hooney.net/?p=712
permalink: /post/712
categories:
  - 웹 디자인
---
어제 Google I/O에서 오픈소스 비디오 포맷인 웹M을 발표한 것에 세간의 시선이 집중됐는데, 한편으로 조용히 [Font API](http://googlecode.blogspot.com/2010/05/introducing-google-font-api-google-font.html)도 공개됐습니다.

<img class="left" src="/wp-content/uploads/2010/05/font_api_logo_beta.gif" alt=" Google Font API" width="196" height="40" /> 

사용 방법은 Font API > [시작하기](http://code.google.com/intl/ko/apis/webfonts/docs/getting_started.html)에서 확인할 수 있습니다. 저도 테스트 해봤는데, 정말 쉽습니다. [폰트 디렉토리](https://fonts.google.com/)도 확인해 보세요.

웹폰트를 지원하는 최근 브라우저에서 사용할 수 있는데, <del datetime="2010-05-25T00:37:35+00:00">테스트 결과 IE6을 포함한</del> Chrome, Firefox, Opera, Safari 최신 버전에도 정상적으로 동작합니다. 제가 만든 [예제](/test/webfont/Google-Font-API.html)를 확인해 보세요.

지난 테스트에 오류가 있었습니다. 현재 IE 계열은 Font linking이나 WOFF fonts를 지원하지 않으며, EOT fonts만 지원합니다. 자세한 테스트 결과는 W3C 국제화 그룹의 [Test results: Webfonts](http://www.w3.org/International/tests/tests-html-css/tests-webfonts/results-webfonts)라는 글을 확인해주세요. WOFF fonts에 대한 설명과 대응 방법은 [Bulletproof @font-face syntax](http://paulirish.com/2009/bulletproof-font-face-implementation-syntax/)에서 확인할 수 있습니다. (최종 수정일: 2010-05-25)

이는 오픈 소스가 **코드**와 **콘텐츠**를 넘어서 **디자인** 영역까지 확대되고 있음을 보여주는 상징적인 의미가 큽니다. 기존에도 공개형 디자인 테마/스킨이나 아이콘 세트 및 레이아웃 가이드처럼 오픈 디자인, 오픈 웹 디자인과 관련된 여러 활동들이 있어왔지만, 관련 정보가 분산되어 있어서 이를 수집하고 정리하는데 어려움이 많았습니다. 그런 측면에서 Google의 Font API는 오픈 소스 디자인의 배포와 활용이라는 점에서 획기적인 변화를 주었다고 볼 수 있습니다.

현재 표준안으로 작업중인 [CSS3는 웹폰트를 정식으로 지원할 예정](http://www.w3.org/TR/css3-fonts/#the-font-face-rule)이지만, 폰트 라이센스 문제에 대해선 딱히 방안을 내놓지 못하고 있습니다. 현재 웹페이지에 사용된 사진이나 이미지에 대한 저작권 사냥(?!)이 횡횡하는 것처럼,  아마 5년 뒤엔 웹폰트에 대한 저작권 사냥이 횡횡할 수 있습니다. 이런 측면에서 구글의 Font API는 웹 디자이너들이 맘 편히 디자인할 수 있는 여건을 만드는 데 일조했다고 볼 수 있습니다.

불필요한 이미지를 제거하고 텍스트를 효과적으로 사용하는 것은 &#8220;**하나의 웹을 보다 소중히 다루고 아름답게 가꾸는 일**&#8220;에 동참하는 가장 쉽고도 큰 일입니다. 부수적으로 접근성도 향상됩니다.  아직 한글 글꼴이 제공되지 않아서 사용하기 어렵지만, 국내 웹 디자이너들이 한 목소리로 요구한다면 한글 글꼴도 제공되지 않을까요? MS가 웹 개발자들의 요구로 IE를 업그레이드했던 것처럼요. 구글 코리아에 한석봉 동화책이라도 보내야 겠군요.