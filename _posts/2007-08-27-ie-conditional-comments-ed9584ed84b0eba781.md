---
id: 451
title: IE Conditional Comments 필터링
date: 2007-08-27T13:45:03+09:00
author: Hooney
layout: post
guid: http://hooney.net/2007/08/27/451/
permalink: /post/451
categories:
  - 웹 접근성
  - 코드
---
W3C의 규격에 의거하여 CSS 코드를 작성하더라도, 각각의 웹 브라우저마다 웹 페이지가 다르게 출력되는 문제가 있습니다. 이러한 문제는 브라우저들이 CSS 규격을 조금씩 서로 다르게 해석하고 출력할 뿐더러, 몇몇 규격은 전혀 출력하지 못하기 때문에 발생합니다.

이처럼 브라우저가 CSS를 W3C 규격과 다르게 출력하거나, 전혀 출력하지 못하는 문제를 CSS 출력 버그(CSS Rendering Bug)라고 합니다. CSS 출력 버그는 표준을 준수하여 웹 페이지를 제작할 때 가장 큰 걸림돌이 됩니다. W3C 규격 외에도 각각의 웹 브라우저들의 CSS 출력 현황에 대해서도 이해해야 하며, 이러한 버그들을 잡는 방법까지 파악해야 하기 때문입니다.

IE7, FF1~2, Opera9, Safari처럼 최근에 출시된(morden) 웹 브라우저들은 W3C 규격에 맞춰서 CSS를 출력합니다. 문제는 IE6, NN7 이하의 오래된 브라우저들이죠. 특히 높은 브라우저 시장 점유율을 기록중인 IE6 브라우저의 CSS 출력 버그들이 큰 문제입니다.

이러한 CSS 출력 버그들을 [CSS Hack](http://centricle.com/ref/css/filters/)과 Filtering으로 대처할 수 있습니다. 예전에는 CSS Hack을 많이 사용했으나, IE7이 출시된 이후로는 CSS Filtering을 주로 사용합니다. 특히 사용이 간단하고 MS에서 추천하는 방법인 IE Conditional Comments Filtering(IE CC-필터링)을 가장 많이 사용합니다.

## IE CC-필터링 소개

IE Conditional Comments은 MS에서 제시한 방법으로 MS IE5 이상의 브라우저에서 사용할 수 있습니다. 이 방법을 이용하면 IE 버전에 따라 HTML 코드를 숨기거나 보일 수 있습니다. 사용자의 IE 버전 별 조건(Condition)을 HTML의 주석(comments)의 구조로 필터링하는 방법기에 IE-CC 필터링이라고 하며, 간단하게 IE-CCF라고 합니다.

아래의 코드를 이용하면 ie7only.css를 IE7에서만 사용할 수 있습니다.

    <!--[if IE 7]>
<link rel="stylesheet" type="text/css" href="ie7only.css">
<![endif]-->

## IE CC-필터링을 사용하는 이유

IE6 이하의 브라우저는 CSS 선택자(selector)에 접근하지 못하는 문제가 있습니다. 이 점을 이용해서 IE6 이하의 브라우저에 특정한 CSS를 추가하거나 숨기는 방법이 바로 CSS Hack입니다. 하지만 CSS2 규격에 정의된 대부분의 선택자를 이용할 수 있는 IE7이 출시되면서, 기존에 사용해왔던 대부분의 CSS Hack들 사용할 수 없게 됐습니다. 이 때문에 최근엔 대부분 웹 개발자와 디자이너들이 브라우저의 CSS 출력 버그를 대처하기 위해서 CSS Filer를 사용합니다.

물론, IE CC-필터링은 HTML에 문법에 맞지 않고 불필요한 코드를 추가하는 문제점이 있습니다. 이에 어떤 개발자는 JS를 이용해서 브라우저의 종류와 버전을 판별하는 방법을 이용하기도 합니다. 하지만 JS를 이용한 방법은 IE CC-필터링보다 코드가 길고 복잡할 뿐더러, DOM으로 접근하기엔 브라우저 파싱 순서가 늦어서 출력되는데 문제가 발생합니다. 즉, CSS 출력 버그를 처리하는데 IE CC-필터링이 최선은 아니지만, 현재로써 가장 확실한 차선책입니다.

## IE CC-필터링 사용법

IE Conditional Comments은 HTML 주석 구조에, IE의 조건문을 포함합니다. IE 조건문은 IE의 버전과 상하관계, 부정조건 등을 사용할 수 있습니다.

    <!--[if 조건]>HTML 코드<![endif]-->

### [조건문에 사용할 수 있는 요소](http://msdn2.microsoft.com/en-us/library/ms537512.aspx#syntax)

<table class="tR">
  <tr>
    <th>
      Item
    </th>
    
    <th>
      Example
    </th>
    
    <th>
      Comment
    </th>
  </tr>
  
  <tr>
    <td>
      IE
    </td>
    
    <td>
      [if IE]
    </td>
    
    <td>
      The only currently supported feature is the string "IE", corresponding to Internet Explorer.
    </td>
  </tr>
  
  <tr>
    <td>
      value
    </td>
    
    <td>
      [if IE 7]
    </td>
    
    <td>
      An integer or floating point numeral corresponding to the version of the browser. Returns a Boolean value of true if the version number matches the browser version. For more information, see <a href="http://msdn2.microsoft.com/en-us/library/ms537512.aspx#Version_Vectors">Version Vectors</a>.
    </td>
  </tr>
  
  <tr>
    <td>
      !
    </td>
    
    <td>
      [if !IE]
    </td>
    
    <td>
      The NOT operator. This is placed immediately in front of the feature, operator, or expression to reverse the Boolean meaning of the expression.
    </td>
  </tr>
  
  <tr>
    <td>
      lt
    </td>
    
    <td>
      [if lt IE 5.5]
    </td>
    
    <td>
      The less-than operator. Returns true if the first argument is less than the second argument.
    </td>
  </tr>
  
  <tr>
    <td>
      lte
    </td>
    
    <td>
      [if lte IE 6]
    </td>
    
    <td>
      The less-than or equal operator. Returns true if the first argument is less than or equal to the second argument.
    </td>
  </tr>
  
  <tr>
    <td>
      gt
    </td>
    
    <td>
      [if gt IE 5]
    </td>
    
    <td>
      The greater-than operator. Returns true if the first argument is greater than the second argument.
    </td>
  </tr>
  
  <tr>
    <td>
      gte
    </td>
    
    <td>
      [if gte IE 7]
    </td>
    
    <td>
      The greater-than or equal operator. Returns true if the first argument is greater than or equal to the second argument.
    </td>
  </tr>
  
  <tr>
    <td>
      ( )
    </td>
    
    <td>
      [if (IE 7)]
    </td>
    
    <td>
      Subexpression operators. Used in conjunction with boolean operators to create more complex expressions.
    </td>
  </tr>
  
  <tr>
    <td>
      &
    </td>
    
    <td>
      [if (gt IE 5)&(lt IE 7)]
    </td>
    
    <td>
      The AND operator. Returns true if all subexpressions evaluate to true
    </td>
  </tr>
  
  <tr>
    <td>
      |
    </td>
    
    <td>
      [if (IE 6)|(IE 7)]
    </td>
    
    <td>
      The OR operator. Returns true if any of the subexpressions evaluates to true.
    </td>
  </tr>
  
  <tr>
    <td>
      true
    </td>
    
    <td>
      [if true]
    </td>
    
    <td>
      Always evaluates to true.
    </td>
  </tr>
  
  <tr>
    <td>
      false
    </td>
    
    <td>
      [if false]
    </td>
    
    <td>
      Always evaluates to false.
    </td>
  </tr>
</table>

### IE CC-필터링 예제

#### IE7일 경우 ie7only.css를 사용

    <!--[if IE 7]>
  <link rel="stylesheet" type="text/css"  href="ie7only.css">
<![endif]-->

#### IE이 아닐 경우 non-ie.css를 사용

    <![if !IE]>
      <link rel="stylesheet" type="text/css"  href="non-ie.css">
    <![endif]>

#### IE7 이하일 경우 ieOld.css를 사용

    <!--[if lt IE7]>
  <link rel="stylesheet" type="text/css" href="ieOld.css">
<![endif]-->

#### IE일 경우 ie.js를 사용하고, IE7 이하일 경우 ie-old.css를 사용

    <![if IE]>
    	
    	<!--[if lt IE7]>
		<link rel="stylesheet" type="text/css" href="ie-old.css">
	<![endif]-->
    <![endif]-->

위에서 소개한 IE CC-필터링 외에도, 다양한 방법의 필터링 방법이 있습니다. [Communis](http://www.communis.co.uk/dithered/css_filters/index.html)에서 CSS만을 이용하거나, HTML을 함께 이용하거나, 또는 JS를 이용하여 필터링하는 방법을 확인할 수 있습니다.

  * [CSS filtering using CSS only](http://www.communis.co.uk/dithered/css_filters/css_only/index.html)
  * [CSS filtering using (X)HTML](http://www.communis.co.uk/dithered/css_filters/html_only/index.html)
  * [CSS filtering using Javascript](http://www.communis.co.uk/dithered/css_filters/js_summary.html)
  * [Non-validating Hacks](http://www.communis.co.uk/dithered/css_filters/nonvalidating/index.php)

## 참고 URI

  * [MSDN : About Conditional Comments](http://msdn2.microsoft.com/en-us/library/ms537512.aspx)
  * [QuirksMode : Conditional comments](http://www.quirksmode.org/css/condcom.html)
  * [Wikipedia : CSS filter](http://en.wikipedia.org/wiki/CSS_filter)
  * [Centricle : CSS filters Table](http://centricle.com/ref/css/filters/)
  * [WaSP : IE7 Conditional Comments](http://www.webstandards.org/2005/11/03/ie7-conditional-comments/)