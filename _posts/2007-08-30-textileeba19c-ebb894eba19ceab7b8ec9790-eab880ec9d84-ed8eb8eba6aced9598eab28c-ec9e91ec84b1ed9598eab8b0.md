---
id: 461
title: Textile로 블로그에 글을 편리하게 작성하기
date: 2007-08-30T15:07:11+09:00
author: Hooney
layout: post
guid: http://hooney.net/2007/08/30/461/
permalink: /post/461
categories:
  - Uncategorized
---
최근 많은 사람들이 블로그를 이용해서 자신의 글을 웹에 기록/공유하고 있습니다. 이 때문에 책보다 블로그에서 양질을 글을 쉽고 빠르게 찾기도 합니다. 실제로 인터넷에서 검색하면 &#8220;구글(Google)&#8221;:http://google.com이나 &#8220;위키피디아(WikiPedia)&#8221;:http://en.wikipedia.org/에서 필요한 내용을 바로 찾아볼 수 있습니다.

좋은 글은 내용이 좋아야 합니다. 그리고 구조적이어야 합니다. 즉, 좋은 웹 문서란 좋은 내용이 잘 구성된 문서입니다. 물론 시각적인 요소나 동적인 효과도 무시할 수 없는 요소이지만, 문서의 핵심은 내용과 구조입니다.

결국, HTML 마크업을 잘 사용해야만 좋은 글을 좋은 웹 문서로 만들 수 있습니다. 제목글에는 h1~h6 태그를, 문단에는 p를, 목록은 ul이나 ol로 구성해야 합니다. 문장이나 단어를 강조하려고 색상을 사용한다면, @<font color="#red">@ 보다 @<stong>@ 태그와 CSS에서 @strong{color:red;}@로 구조와 표현을 분리해야 합니다.</p> 

<p>
  아무리 HTML이 쉽다고 하더라도, 블로그에 글을 작성하는 사람들 중에선 HTML을 거의 사용할 줄 모르는 분이 더 많습니다. 수 많은 실무 웹 종사자들도 HTML을 올바르게 작성하는 게 어려운 현실이죠. 이 때문에 많은 블로거들이 이지윅(WYSIWYG) 에디터를 사용하고 있습니다. 하지만 이지웍 에디터가 최선의 대안일까요?
</p>

<p>
  h2. Textile 소개
</p>

<p>
  Textile은 &#8220;humane Web text generator&#8221;라는 목적으로 &#8220;Dean Allen&#8221;:http://textism.com/about/이 만든 경량의 마크업 언어입니다. 위키 마크업처럼 별표(*)나 대시(-), 인용부호(&#8216;) 등을 구조화된 HTML으로 변경시켜줍니다. 또한 &#8220;<, >&#8221; 부등호를 &#8220;<, >&#8221;로 인코딩하기 때문에 HTML 코드를 블로그에 작성하기 편리합니다. Textile에 대한 자세한 내용은 &#8220;위키피디아&#8221;:http://en.wikipedia.org/wiki/Textile_%28markup_language%29에서 확인할 수 있습니다.
</p>

<p>
  bq. Textile is a lightweight markup language originally developed by Dean Allen and billed as a &#8220;humane Web text generator&#8221;. Textile converts its marked-up text input to valid, well-formed XHTML and also inserts character entity references for apostrophes, opening and closing single and double quotation marks, ellipses and em dashes. -위키피디아
</p>

<p>
  h2. Textile 문법
</p>

<p>
  |_. 화면 출력 |_. HTML |_. Textile |<br /> |
</p>

<h1>
  첫번째 제목글</p> 
  
  <h1>
    | @</p> 
    
    <h1>
      첫번째 제목글</p> 
      
      <h1>
        @ | @h1. 첫번째 제목글@ |<br /> | </p> 
        
        <h2>
          두번째 제목글</p> 
          
          <h2>
            | @</p> 
            
            <h2>
              두번째 제목글</p> 
              
              <h2>
                @ | @h2. 두번째 제목글@ |<br /> | </p> 
                
                <h3>
                  세번째 제목글</p> 
                  
                  <h3>
                    | @</p> 
                    
                    <h3>
                      세번째 제목글</p> 
                      
                      <h3>
                        @ | @h3. 세번째 제목글@ |<br /> | </p> 
                        
                        <p>
                          문단
                        </p>
                        
                        <p>
                          | @
                        </p>
                        
                        <p>
                          문단
                        </p>
                        
                        <p>
                          @ | 문단 |<br /> |
                        </p>
                        
                        <ol>
                          <li>
                            순서 있는 목록
                          </li>
                        </ol>
                        
                        <p>
                          | @
                        </p>
                        
                        <ol>
                          <li>
                            순서 있는 목록
                          </li>
                        </ol>
                        
                        <p>
                          @ | @# 순서있는 목록@ |<br /> |
                        </p>
                        
                        <ul>
                          <li>
                            순서 없는 목록
                          </li>
                        </ul>
                        
                        <p>
                          | @
                        </p>
                        
                        <ul>
                          <li>
                            순서 없는 목록
                          </li>
                        </ul>
                        
                        <p>
                          @ | @* 순서없는 목록@ |<br /> | @code@ | @<code>code</code>@ | <code>@code@</code> |<br /> | <em>강조</em> | @<em>강조</em>@ | @_강조_@ |<br /> | <strong>더욱강조</strong> | @<strong>더욱강조</strong>@ | @*더욱강조*@ |<br /> | <a href="/url">연결</a> | @<a href="/url">연결</a>@ | @&#8221;연결&#8221;:/url@ |
                        </p>
                        
                        <p>
                          이 외에도 &#8220;다양한 문법&#8221;:http://hobix.com/textile/을 사용할 수 있으며, 또한 &#8220;Textism&#8221;:http://textism.com/tools/textile/에서 연습할 수도 있습니다.
                        </p>
                        
                        <p>
                          h2. Textile 플러그인
                        </p>
                        
                        <p>
                          &#8220;텍스트패턴&#8221;:http://www.textpattern.com/은 Textile을 기본적으로 사용할 수 있으며, 이 외 블로그 툴은 플러그인을 설치해서 사용할 수 있습니다. 아쉽게도 플러그인을 제공하지 않는 서비스형 블로그는 서비스 회사의 지원 없이는 사용할 수 없겠네요.
                        </p>
                        
                        <p>
                          * &#8220;워드프레스(WordPress) Textile 플러그인&#8221;:http://idly.org/category/textile<br /> * &#8220;무버블타입(MovableType) Textile 플러그인&#8221;:http://www.bradchoate.com/mt-plugins/textile
                        </p>
                        
                        <p>
                          h2. 유사한 마크업 언어
                        </p>
                        
                        <p>
                          * &#8220;Wiki markup&#8221;:http://en.wikipedia.org/wiki/Wikipedia:Formatting#Wiki_Markup<br /> * &#8220;MarkDown&#8221;:http://daringfireball.net/projects/markdown/<br /> * 관련 정보를 제공해주세요~
                        </p>