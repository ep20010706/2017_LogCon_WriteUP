# #11. [300]고대의 웹사이트: the_world_wide_web_project
문제:
팀 버너스리는 HTML을 최초로 만든 뛰어난 양자물리학자이자 최초의 웹 개발자입니다.
그는 1989년 글로벌 하이퍼텍스트 프로젝트를 제안하였고, 1990년 최초의 하이퍼텍스트 브라우저와 편집기를 개발하였으며 1991년에는 최초의 웹 페이지를 만들었습니다.
이후로도 여러 가지의 업적을 남겼으며 현재까지 차세대 웹 기술인 시맨틱 웹 기술 표준화에 힘을 쏟고 있는 중입니다.

이 팀 버너스리가 만들었던 최초의 웹사이트에서 <title> 태그에 들어가있는 문장은 무엇일까요?

Hint : <title> 태그는 웹브라우저 창(탭)의 제목 표시줄, 작업 표시줄에 표시되는 태그입니다.

풀이:
https://goo.gl/8JDdNL 에 가면 최초의 웹사이트의 모습을 볼 수 있다. 다음은 최초의 웹사이트에서의 소스코드의 일부분이다.
```
<HEADER>
<TITLE>The World Wide Web project</TITLE>
<NEXTID N="55">
</HEADER>
<BODY>
<H1>World Wide Web</H1>The WorldWideWeb (W3) is a wide-area<A
NAME=0 HREF="WhatIs.html">
hypermedia</A> information retrieval
initiative aiming to give universal
access to a large universe of documents.<P>
Everything there is online about
W3 is linked directly or indirectly
to this document, including an <A
NAME=24 HREF="Summary.html">executive
summary</A> of the project, <A
```
여기서 <TITLE>태그 안에 The World Wide Web project라는 문장이 들어있는 것을 확인할 수 있다.
Flag는 the_world_wide_web_project다.

# #12. [500]질빼기 타입: <!doctype_html_public_"-//ietf//dtd_html_2.0//en">
문제:
HTML은 여러 가지의 버전이 있습니다.
대부분의 HTML 문서에는 약속적으로 코드 가장 윗줄에 HTML의 버전을 알리는 '이것'을 함께 작성해 놓습니다.
버전을 알 수 있는 '이것'은 HTML5 버전부터 길이가 굉장히 짧아졌습니다.
HTML이 가장 처음 표준화되었을 때의 버전에서 '이것'의 코드 작성하세요.

풀이:
최초로 HTML의 표준이 발표된 것은 1995년 11월 24일 HTML 2.0이 IETF의 RFC 1866로 발표된 것으로 웹 표준화가 시작되었다.
다음은 HTML 2.0으로 작성된 웹페이지 소스의 일부분이다.
```
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<HTML>
<HEAD>
  <TITLE>HTML 2.0 Materials</TITLE>
</HEAD>
<BODY>
<P>
<A HREF="../../"> <IMG ALT="WWW" SRC="../../Icons/WWW/WWWlogo48.gif"></A>
<A HREF="../"> <IMG ALT="HTML" SRC="../../Icons/WWW/html_48x48.gif"></A>
<H1>
  <A HREF="http://validator.w3.org/check?uri=http://www.w3.org/MarkUp/html-spec/"><IMG
      SRC="../valid_html.gif" ALT="HTML 2.0 Check" ></A>HTML 2.0 Materials
</H1>
<P>
The HTML 2.0 specification <A href="http://www.ietf.org/rfc/rfc1866.txt">RFC
1866</A>, is a product of the <A HREF="../HTML-WG/Overview.html"> HTML Working
Group</A> of the
<A href="http://www.ietf.cnri.reston.va.us/home.html">IETF</A>, edited by
<A href="../../People/Connolly/">Dan Connolly</A>.
```
HTML은 doctype를 이용하여 버전을 구분한다.
그러므로 Flag는 <!doctype_html_public_"-//ietf//dtd_html_2.0//en">이다.

# #13. [100]손 보는 성윤: killall5
문제:


풀이:


# #14. [100]감시자: who
문제:


풀이:


# #15. [100]잡담: write_sh
문제:


풀이:

