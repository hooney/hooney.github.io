---
id: 266
title: 중/대형 웹사이트 기획 팁
date: 2006-04-26T11:23:11+09:00
author: Hooney
layout: post
guid: http://hooney.net/wp/?p=266
permalink: /post/266
keywords:
  - CSS,기획
categories:
  - 웹 디자인
---
웹사이트의 목표와 방향을 설정하고 컨텐츠들을 정리/분배할 때, 각 컨텐츠 집합들을 아이템화(공식어는 모듈화인듯)한다. 그 후 각각의 아이템 집합들에 2가지 인식자(심볼/기호)을 부여하여 사이트 전체적인 일관성과 개별 아이템의 개별성을 꾀한다. 

2가지 인식자는 class라는 공용(범용) 심볼과 id라는 전용 심볼로 구성되는데, 각각의 아이템에 포함된 컨텐츠의 의미와 구성, 그리고 보여질 디자인 패턴을 감안하여 부여한다.

인식자를 표기할 때 전제조건은 한글이 아닌 영문으로, 대문자를 포함하지 않은 소문자와 &#8211; 또는 _ 를 사용하여 표기하는 것이다.

이렇게 기획안을 구성하면, 웹사이트의 컨텐츠들을 빠짐없이 정리/분배할 수 있으며, 사이트 전체적인 흐름을 파악하고 컨텐츠를 구성하는데 편리하다. 이는 기획안을 작성하는 기획자 자신에겐 업무 효율성을 증대시킬 뿐만 아니라, 기획안을 보는 다른 이들도 기획자의 의도를 쉽게 파악할 수 있다. 즉, 웹디자이너는 기획안에 표기된 공용/전용 인식자들을 토대로 웹디자인을 하게될 것이며, 웹퍼블리셔(코더)는 xhtml/css를 개발할 것이다. 무척 효율적인 작업 흐름이지 않은가?

그렇다. 이 방법은 (x)html를 제작할 때, class/id 선택자를 이용하여 각 컨텐츠를 모듈화하고, 이들 모듈을 css로 디자인하는 과정을 기획단계로 확장시킨 것이다. 물론 이와 같거나 비슷한 방법을 사용하는 많은 웹사이트 개발사가 존재하고 있을 것이다. 또는 더 효율적인 방법을 사용하는 곳이 있을 것이다. 하지만, 아직 많은 개발사가 체계적이지 못한 기획안을 작성하고, 이를 디자인하며 개발하고 있을 것이다.

웹사이트의 컨텐츠를 모듈화하고, 각 모듈에 적절한 인식자를 부여하는 것만으로도 기획안의 성공을 50% 이상 좌우할 것이라고 믿는다. ㅎㅎ

참고로 이 방법은 소형 웹사이트를 개발할 때도 이용할 수 있겠지만, 중/대형 웹사이트를 개발할 때 더욱 효율적일 것이다. 다음 글은 웹디자인에 있어서 스타일 가이드 작성에 대해 짧게 이야기할 생각임. ^^