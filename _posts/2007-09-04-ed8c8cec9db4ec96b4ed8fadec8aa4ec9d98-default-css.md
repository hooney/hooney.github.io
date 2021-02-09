---
id: 479
title: 파이어폭스의 default CSS
date: 2007-09-04T23:54:16+09:00
author: Hooney
layout: post
guid: http://hooney.net/2007/09/04/479/
permalink: /post/479
categories:
  - CSS
  - 웹 접근성
---
웹 브라우저마다 각각 default CSS가 존재합니다. cascade한 CSS의 특성상, 제작자가 작성한 CSS도 브라우저의 디폴트 CSS의 영향을 받습니다. 웹 사이트가 브라우저마다 조금씩 다르게(경우에 따라 심각하게) 표현되는 이유가 바로 default CSS 때문입니다.

[<img src="/wp-content/uploads/2007/09/css2.gif" width="511" height="311" alt="css cascade" class="imageframe" />](/wp-content/uploads/2007/09/css2.gif "css cascade"){.thickbox}

W3C에서 예제로 보여준 default CSS와 파이어폭스(FireFox)의 default CSS, 그리고 Quirks 모드에서 default CSS를 비교함으로써, 다양한 브라우저들의 default CSS를 보다 쉽게 이해할 수 있습니다. 아쉽게도 windows 환경에서 IE와 Opera, Safari는 dll 파일 형식으로 작성되어 확인하기 어렵네요.

## default CSS의 위치/경로

  * [W3C의 default CSS &#8211; http://www.w3.org/TR/CSS21/sample.html](http://www.w3.org/TR/CSS21/sample.html)
  * 파이어폭스의 default CSS &#8211; C:\Program Files\Mozilla Firefox\res\html.css (windows xp)
  * 파이어폭스의 Quirks 모드에서 default CSS &#8211; C:\Program Files\Mozilla Firefox\res\quirks.css (windows xp)

## W3C의 default CSS

<pre>html, address, blockquote, body, dd, div, dl, dt, fieldset, form, frame, frameset, h1, h2, h3, h4, h5, h6, noframes, ol, p, ul, center, dir, hr, menu, pre { display: block }
li { display: list-item }
head { display: none }
table { display: table }
tr { display: table-row }
thead { display: table-header-group }
tbody { display: table-row-group }
tfoot { display: table-footer-group }
col { display: table-column }
colgroup { display: table-column-group }
td, th { display: table-cell }
caption { display: table-caption }
th { font-weight: bolder; text-align: center }
caption { text-align: center }
body { margin: 8px }
h1 { font-size: 2em; margin: .67em 0 }
h2 { font-size: 1.5em; margin: .75em 0 }
h3 { font-size: 1.17em; margin: .83em 0 }
h4, p, blockquote, ul, fieldset, form, ol, dl, dir, menu { margin: 1.12em 0 }
h5 { font-size: .83em; margin: 1.5em 0 }
h6 { font-size: .75em; margin: 1.67em 0 }
h1, h2, h3, h4, h5, h6, b, strong { font-weight: bolder }
blockquote { margin-left: 40px; margin-right: 40px }
i, cite, em, var, address { font-style: italic }
pre, tt, code, kbd, samp { font-family: monospace }
pre { white-space: pre }
button, textarea, input, select { display: inline-block }
big { font-size: 1.17em }
small, sub, sup { font-size: .83em }
sub { vertical-align: sub }
sup { vertical-align: super }
table { border-spacing: 2px; }
thead, tbody, tfoot { vertical-align: middle }
td, th { vertical-align: inherit }
s, strike, del { text-decoration: line-through }
hr { border: 1px inset }
ol, ul, dir, menu, dd { margin-left: 40px }
ol { list-style-type: decimal }
ol ul, ul ol, ul ul, ol ol { margin-top: 0; margin-bottom: 0 }
u, ins { text-decoration: underline }
br:before { content: "\A" }
:before, :after { white-space: pre-line }
center { text-align: center }
:link, :visited { text-decoration: underline }
:focus { outline: thin dotted invert }
/* Begin bidirectionality settings (do not change) */
BDO[DIR="ltr"] { direction: ltr; unicode-bidi: bidi-override }
BDO[DIR="rtl"] { direction: rtl; unicode-bidi: bidi-override }
*[DIR="ltr"] { direction: ltr; unicode-bidi: embed }
*[DIR="rtl"] { direction: rtl; unicode-bidi: embed }
 @media print {
h1 { page-break-before: always }
h1, h2, h3,  h4, h5, h6 { page-break-after: avoid }
ul, ol, dl { page-break-before: avoid }
}</pre>

## 파이어폭스(FireFox)의 default CSS (windows xp)

<pre>*|:-moz-any-link img, img[usemap], object[usemap] {
border:2px solid;
}
[dir=ltr] {
direction:ltr;
unicode-bidi:embed;
}
[dir=rtl] {
direction:rtl;
unicode-bidi:embed;
}
abbr:focus, acronym:focus, address:focus, applet:focus, b:focus, base:focus, big:focus, blockquote:focus, br:focus, canvas:focus, caption:focus, center:focus, cite:focus, code:focus, col:focus, colgroup:focus, dd:focus, del:focus, dfn:focus, dir:focus, div:focus, dl:focus, dt:focus, em:focus, fieldset:focus, font:focus, form:focus, h1:focus, h2:focus, h3:focus, h4:focus, h5:focus, h6:focus, hr:focus, i:focus, img:focus, ins:focus, kbd:focus, label:focus, legend:focus, li:focus, link:focus, menu:focus, object:focus, ol:focus, p:focus, pre:focus, q:focus, s:focus, samp:focus, small:focus, span:focus, strike:focus, strong:focus, sub:focus, sup:focus, table:focus, tbody:focus, td:focus, tfoot:focus, th:focus, thead:focus, tr:focus, tt:focus, u:focus, ul:focus, var:focus { outline:1px dotted invert; }
abbr[title], acronym[title] { border-bottom:dotted 1px; }
address { display:block; font-style:italic; }
area, base, basefont, head, meta, script, style, title, noembed, param { display:none; }
b, strong { font-weight:bolder; }
bdo[dir] { unicode-bidi:bidi-override; }
big { font-size:larger; }
blink { text-decoration:blink; }
blockquote { display:block; margin:1em 40px; }
blockquote[type=cite] { border-color:blue; border-left:solid; border-width:thin; display:block; margin:1em 0; padding-left:1em; }
body { display:block; margin:8px; }
canvas { -moz-user-select:none; }
caption { -moz-box-sizing:border-box; display:table-caption; text-align:center; }
center { display:block; text-align:0; }
col { display:table-column; }
colgroup { display:table-column-group; }
dd { -moz-margin-start:40px; display:block; }
frame { border:none!important; }
frameset { border:none!important; display:block!important; float:none!important; overflow:0; position:static!important; }
h1 { display:block; font-size:2em; font-weight:bold; margin:.67em 0; }
h2 { display:block; font-size:1.5em; font-weight:bold; margin:.83em 0; }
h3 { display:block; font-size:1.17em; font-weight:bold; margin:1em 0; }
h4 { display:block; font-weight:bold; margin:1.33em 0; }
h5 { display:block; font-size:.83em; font-weight:bold; margin:1.67em 0; }
h6 { display:block; font-size:.67em; font-weight:bold; margin:2.33em 0; }
hr { -moz-box-sizing:border-box; -moz-float-edge:margin-box; border:1px 0; display:block; height:2px; margin:.5em auto; }
 hr[size=1] {
border-style:0 none none;
}
html, div, map, dt, isindex, form { display:block; }
i, cite, em, var, dfn { font-style:italic; }
iframe { border:2px inset; }
img[usemap], object[usemap] { color:blue; }
li { -moz-float-edge:margin-box; display:list-item; }
listing { display:block; font-family:0; font-size:medium; margin:1em 0; white-space:pre; }
marquee { -moz-binding:url(chrome://xbl-marquee/content/xbl-marquee.xml#marquee-horizontal); display:block; }
marquee[direction=up], marquee[direction=down] { -moz-binding:url(chrome://xbl-marquee/content/xbl-marquee.xml#marquee-vertical); height:200px; }
nobr { white-space:nowrap; }
noframes { display:none; }
ol { -moz-padding-start:40px; display:block; list-style-type:decimal; margin:1em 0; }
ol ol ul, ol ul ul, ol menu ul, ol dir ul, ol ol menu, ol ul menu, ol menu menu, ol dir menu, ol ol dir, ol ul dir, ol menu dir, ol dir dir, ul ol ul, ul ul ul, ul menu ul, ul dir ul, ul ol menu, ul ul menu, ul menu menu, ul dir menu, ul ol dir, ul ul dir, ul menu dir, ul dir dir, menu ol ul, menu ul ul, menu menu ul, menu dir ul, menu ol menu, menu ul menu, menu menu menu, menu dir menu, menu ol dir, menu ul dir, menu menu dir, menu dir dir, dir ol ul, dir ul ul, dir menu ul, dir dir ul, dir ol menu, dir ul menu, dir menu menu, dir dir menu, dir ol dir, dir ul dir, dir menu dir, dir dir dir { list-style-type:square; }
ol ul, ul ul, menu ul, dir ul, ol menu, ul menu, menu menu, dir menu, ol dir, ul dir, menu dir, dir dir { list-style-type:circle; }
p, dl, multicol { display:block; margin:1em 0; }
pre[_moz_quote=true] { color:blue; }
q:after { content:close-quote; }
q:before { content:open-quote; }
s, strike, del { text-decoration:line-through; }
small { font-size:smaller; }
spacer { float:none!important; position:static!important; }
span[_moz_quote=true] { color:blue; }
sub { font-size:smaller; line-height:normal; vertical-align:sub; }
sup { font-size:smaller; line-height:normal; vertical-align:super; }
table { -moz-box-sizing:border-box; border-collapse:separate; border-spacing:2px; display:table; margin-bottom:0; margin-top:0; text-indent:0; }
table > tr { vertical-align:middle; }
table[align=center] > caption { margin-left:auto; margin-right:auto; }
table[align=center] > caption[align=left] { margin-right:0; }
table[align=center] > caption[align=right] { margin-left:0; }
table[align=left] { float:left; }
table[align=right] { float:right; text-align:start; }
 table[rules]:not([rules=none]) {
border-collapse:collapse;
}
tbody { display:table-row-group; vertical-align:middle; }
td { display:table-cell; padding:1px; text-align:inherit; vertical-align:inherit; }
tfoot { display:table-footer-group; vertical-align:middle; }
th { display:table-cell; font-weight:bold; padding:1px; vertical-align:inherit; }
thead { display:table-header-group; vertical-align:middle; }
tr { display:table-row; vertical-align:inherit; }
 tr > form:-moz-is-html, tbody > form:-moz-is-html, thead > form:-moz-is-html, tfoot > form:-moz-is-html, table > form:-moz-is-html {
display:none!important;
}
tt, code, kbd, samp { font-family:0; }
u, ins { text-decoration:underline; }
ul ul, ul ol, ul dir, ul menu, ul dl, ol ul, ol ol, ol dir, ol menu, ol dl, dir ul, dir ol, dir dir, dir menu, dir dl, menu ul, menu ol, menu dir, menu menu, menu dl, dl ul, dl ol, dl dir, dl menu, dl dl { margin-bottom:0; margin-top:0; }
ul, menu, dir { -moz-padding-start:40px; display:block; list-style-type:disc; margin:1em 0; }
xmp, pre, plaintext { display:block; font-family:0; margin:1em 0; white-space:pre; }
 @media print {
blink { text-decoration:none; }
marquee { -moz-binding:none; }
}</pre>

## 파이어폭스(FireFox)의 quirks default CSS (windows xp)

<pre>:not(dl) > dd { display:inline; margin:0; }
:not(dl) > dd:before { -moz-margin-end:40px; content:"\A  "; display:inline; font-size:1px; line-height:0; white-space:pre; }
 [_moz-rs-heading] { font-size:inherit!important; }
 body > form:-moz-first-node, td > form:-moz-first-node, th > form:-moz-first-node, body > p:-moz-first-node, td > p:-moz-first-node, th > p:-moz-first-node, body > dl:-moz-first-node, td > dl:-moz-first-node, th > dl:-moz-first-node, body > multicol:-moz-first-node, td > multicol:-moz-first-node, th > multicol:-moz-first-node, body > blockquote:-moz-first-node, td > blockquote:-moz-first-node, th > blockquote:-moz-first-node, body > h1:-moz-first-node, td > h1:-moz-first-node, th > h1:-moz-first-node, body > h2:-moz-first-node, td > h2:-moz-first-node, th > h2:-moz-first-node, body > h3:-moz-first-node, td > h3:-moz-first-node, th > h3:-moz-first-node, body > h4:-moz-first-node, td > h4:-moz-first-node, th > h4:-moz-first-node, body > h5:-moz-first-node, td > h5:-moz-first-node, th > h5:-moz-first-node, body > h6:-moz-first-node, td > h6:-moz-first-node, th > h6:-moz-first-node, body > listing:-moz-first-node, td > listing:-moz-first-node, th > listing:-moz-first-node, body > plaintext:-moz-first-node, td > plaintext:-moz-first-node, th > plaintext:-moz-first-node, body > xmp:-moz-first-node, td > xmp:-moz-first-node, th > xmp:-moz-first-node, body > pre:-moz-first-node, td > pre:-moz-first-node, th > pre:-moz-first-node, body > ul:-moz-first-node, td > ul:-moz-first-node, th > ul:-moz-first-node, body > menu:-moz-first-node, td > menu:-moz-first-node, th > menu:-moz-first-node, body > dir:-moz-first-node, td > dir:-moz-first-node, th > dir:-moz-first-node, body > ol:-moz-first-node, td > ol:-moz-first-node, th > ol:-moz-first-node {
margin-top:0;
}
 body > form:-moz-only-whitespace:-moz-first-node, td > form:-moz-only-whitespace:-moz-first-node, th > form:-moz-only-whitespace:-moz-first-node, body > p:-moz-only-whitespace:-moz-first-node, td > p:-moz-only-whitespace:-moz-first-node, th > p:-moz-only-whitespace:-moz-first-node, body > dl:-moz-only-whitespace:-moz-first-node, td > dl:-moz-only-whitespace:-moz-first-node, th > dl:-moz-only-whitespace:-moz-first-node, body > multicol:-moz-only-whitespace:-moz-first-node, td > multicol:-moz-only-whitespace:-moz-first-node, th > multicol:-moz-only-whitespace:-moz-first-node, body > blockquote:-moz-only-whitespace:-moz-first-node, td > blockquote:-moz-only-whitespace:-moz-first-node, th > blockquote:-moz-only-whitespace:-moz-first-node, body > h1:-moz-only-whitespace:-moz-first-node, td > h1:-moz-only-whitespace:-moz-first-node, th > h1:-moz-only-whitespace:-moz-first-node, body > h2:-moz-only-whitespace:-moz-first-node, td > h2:-moz-only-whitespace:-moz-first-node, th > h2:-moz-only-whitespace:-moz-first-node, body > h3:-moz-only-whitespace:-moz-first-node, td > h3:-moz-only-whitespace:-moz-first-node, th > h3:-moz-only-whitespace:-moz-first-node, body > h4:-moz-only-whitespace:-moz-first-node, td > h4:-moz-only-whitespace:-moz-first-node, th > h4:-moz-only-whitespace:-moz-first-node, body > h5:-moz-only-whitespace:-moz-first-node, td > h5:-moz-only-whitespace:-moz-first-node, th > h5:-moz-only-whitespace:-moz-first-node, body > h6:-moz-only-whitespace:-moz-first-node, td > h6:-moz-only-whitespace:-moz-first-node, th > h6:-moz-only-whitespace:-moz-first-node, body > listing:-moz-only-whitespace:-moz-first-node, td > listing:-moz-only-whitespace:-moz-first-node, th > listing:-moz-only-whitespace:-moz-first-node, body > plaintext:-moz-only-whitespace:-moz-first-node, td > plaintext:-moz-only-whitespace:-moz-first-node, th > plaintext:-moz-only-whitespace:-moz-first-node, body > xmp:-moz-only-whitespace:-moz-first-node, td > xmp:-moz-only-whitespace:-moz-first-node, th > xmp:-moz-only-whitespace:-moz-first-node, body > pre:-moz-only-whitespace:-moz-first-node, td > pre:-moz-only-whitespace:-moz-first-node, th > pre:-moz-only-whitespace:-moz-first-node, body > ul:-moz-only-whitespace:-moz-first-node, td > ul:-moz-only-whitespace:-moz-first-node, th > ul:-moz-only-whitespace:-moz-first-node, body > menu:-moz-only-whitespace:-moz-first-node, td > menu:-moz-only-whitespace:-moz-first-node, th > menu:-moz-only-whitespace:-moz-first-node, body > dir:-moz-only-whitespace:-moz-first-node, td > dir:-moz-only-whitespace:-moz-first-node, th > dir:-moz-only-whitespace:-moz-first-node, body > ol:-moz-only-whitespace:-moz-first-node, td > ol:-moz-only-whitespace:-moz-first-node, th > ol:-moz-only-whitespace:-moz-first-node {
margin-bottom:0;
}
dl > dl { -moz-margin-start:40px; display:block; }
form { margin:0 0 1em; }
img[align=left] { margin-right:3px; }
img[align=right] { margin-left:3px; }
 input:not([type=image]), textarea { -moz-box-sizing:border-box; }
input[type=image] { border:2px solid blue; }
input[type=image][disabled] { border-color:GrayText; }
li { list-style-position:inside; }
 li > ul:-moz-first-node, li > ol:-moz-first-node { padding-top:1em; }
li ul, li ol, li dir, li menu { list-style-position:outside; }
 li::-moz-list-bullet { font-size:0; }
map { display:inline; }
pre[wrap], pre[cols], pre[width] { white-space:0; }
table { font-size:0; font-style:0; font-variant:0; font-weight:0; line-height:normal; text-align:start; white-space:normal; }
 td > form:-moz-only-whitespace:-moz-last-node, th > form:-moz-only-whitespace:-moz-last-node, td > p:-moz-only-whitespace:-moz-last-node, th > p:-moz-only-whitespace:-moz-last-node, td > dl:-moz-only-whitespace:-moz-last-node, th > dl:-moz-only-whitespace:-moz-last-node, td > multicol:-moz-only-whitespace:-moz-last-node, th > multicol:-moz-only-whitespace:-moz-last-node, td > blockquote:-moz-only-whitespace:-moz-last-node, th > blockquote:-moz-only-whitespace:-moz-last-node, td > h1:-moz-only-whitespace:-moz-last-node, th > h1:-moz-only-whitespace:-moz-last-node, td > h2:-moz-only-whitespace:-moz-last-node, th > h2:-moz-only-whitespace:-moz-last-node, td > h3:-moz-only-whitespace:-moz-last-node, th > h3:-moz-only-whitespace:-moz-last-node, td > h4:-moz-only-whitespace:-moz-last-node, th > h4:-moz-only-whitespace:-moz-last-node, td > h5:-moz-only-whitespace:-moz-last-node, th > h5:-moz-only-whitespace:-moz-last-node, td > h6:-moz-only-whitespace:-moz-last-node, th > h6:-moz-only-whitespace:-moz-last-node, td > listing:-moz-only-whitespace:-moz-last-node, th > listing:-moz-only-whitespace:-moz-last-node, td > plaintext:-moz-only-whitespace:-moz-last-node, th > plaintext:-moz-only-whitespace:-moz-last-node, td > xmp:-moz-only-whitespace:-moz-last-node, th > xmp:-moz-only-whitespace:-moz-last-node, td > pre:-moz-only-whitespace:-moz-last-node, th > pre:-moz-only-whitespace:-moz-last-node, td > ul:-moz-only-whitespace:-moz-last-node, th > ul:-moz-only-whitespace:-moz-last-node, td > menu:-moz-only-whitespace:-moz-last-node, th > menu:-moz-only-whitespace:-moz-last-node, td > dir:-moz-only-whitespace:-moz-last-node, th > dir:-moz-only-whitespace:-moz-last-node, td > ol:-moz-only-whitespace:-moz-last-node, th > ol:-moz-only-whitespace:-moz-last-node {
margin-top:0;
}
 td > p:-moz-last-node, th > p:-moz-last-node { margin-bottom:0; }
ul ul, ul ol, ul dir, ul menu, ul li, ol ul, ol ol, ol dir, ol menu, ol li, dir ul, dir ol, dir dir, dir menu, dir li, menu ul, menu ol, menu dir, menu menu, menu li { list-style-position:inherit; }</pre>

위의 CSS 코드는 [Code Beautifier](http://www.codebeautifier.com/)와 드림위버 CS3에서 제공하는 &#8220;코드 포맷 정리&#8221; 기능을 이용해서 정리했습니다. 🙂