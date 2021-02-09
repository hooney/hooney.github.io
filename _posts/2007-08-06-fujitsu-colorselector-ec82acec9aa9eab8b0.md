---
id: 422
title: Fujitsu ColorSelector 사용기
date: 2007-08-06T18:42:32+09:00
author: Hooney
layout: post
guid: http://hooney.net/2007/08/06/422/
permalink: /post/422
categories:
  - 웹 접근성
---
지난 번에 작성한 [Fujitsu 웹 접근성 보조기기](/2007/07/30/417/)를 소개한 글에 이어서 개별 제품들에 대한 사용기를 작성합니다. 그 첫번째로 오늘은 접근성 높은 웹 컬러를 선택하도록 도와주는 Fujitsu ColorSelector에 대한 사용기를 작성합니다.

Fujitsu ColorSelector는 배경색과 전경색을 조합할 때 색약자가 겪을 수 있는 이상유무를 실시간으로 판별해줍니다. 일반, 백내장, 제1색각(빨강), 제2색각(초록), 제3색각(파랑)의 5가지 색약 분류에 따라 이상 유무를 O/X로 판별해주기 때문에 웹 디자이너 입장에서 접근성을 이해하고 활용하는데 무척 유용한 도구입니다.

제가 주로 사용하는 색상선택기인 [ColorCop](/2006/12/26/341/)와 비교하면, 몇가지 불편한 점이 있습니다. 예를 들어, 디자이너가 선택한 전경색과 배경색이 접근성에 문제가 있을 경우에 접근성이 높은 유사한 색상들의 목록을 제공해주지 않고 있습니다. 또한, 색상을 선택하기 위해서 현재의 화면을 팔레트로 사용하는 것이 아니라 스크린캡쳐 받은 영역을 사용하는 문제점이 있습니다. 이 때문에 실시간으로 변경하는 영역의 색생을 선택하는데 불편함이 있습니다.

국내 포털 사이트인 [다음(Daum)의 메인 페이지](http://daum.net/) 중에서 색대비가 약한 부분인 사이트맵 영역의 버튼을 Fujitsu ColorSelector로 점검해봤습니다. 전경색이 #FFFFFF이고 배경색이 #C6C6C6이기에 한눈에 봐도 색약 관련 접근성이 낮겠다고 예상할 수 있겠네요.

<img src="/files/fujitsu/cs/daumSitemap.png" title="다음 메인 페이지의 사이트맵" alt="다음 메인 페이지의 사이트맵" height="135" width="428" /> 

Fujitsu ColorSelector로 점검해보니 제1색각(빨강)을 제외한 일반, 백내장, 제2색각(초록), 제3색각(파랑)의 4가지 영역에서 문제가 있음을 확인할 수 있었습니다.  
<img src="/files/fujitsu/cs/ss.png" title="Fujitsu ColorSelector" alt="Fujitsu ColorSelector" height="660" width="464" /> 

사람이 점검할 때는 많은 시간과 노력이 들면서도 그 결과의 객관성 확보에 문제가 발생하곤 합니다. 특히 웹 접근성 영역이 그러하죠. Fujitsu ColorSelector와 같은 유용한 도구를 이용함으로써 보다 객관적이면서도 쉽고 빠르게 색상과 관련한 웹 접근성을 점검할 수 있습니다.

앞으로도 이와 같은 유용한 도구들이 많이 만들어졌으면 좋겠습니다. 물론 제가 할 수 있는 영역에서 최선을 다할 것이구요. ㅎㅎ

Fujitsu ColorSelector에 대한 자세한 소개는 아래 링크를 참고하세요.

  * [Fujitsu ColorSelector 소개(영문)](http://www.fujitsu.com/global/accessibility/assistance/cs/)
  * [Fujitsu ColorSelector 소개(일한 번역)](http://j2k.naver.com/j2k.php/korean/jp.fujitsu.com/about/design/ud/assistance/colordoctor/)
  * [Fujitsu ColorSelector 다운로드(한글판포함)](http://www.fujitsu.com/global/accessibility/assistance/cs/download.html)
  * [Fujitsu ColorSelector 사용 설명서(한글)](/files/fujitsu/cs/UserGuide_cs_kr.html)