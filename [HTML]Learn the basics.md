# HTML basics

*write by JaeHwanKwon* (21/09/24) <br>
HTML 기초

## 📙 HTML

 *HTML(**H**yper**T**ext**M**arkup**L**anguage)은 웹 페이지와 그 내용을 구조화 하기 위해 사용되는 코드이다*

 * HTML은 프로그래밍 언어가 아니다 <br>

 * 컨텐츠의 구조를 정의하는 마크업 언어이다
 
 * 컨텐츠의 서로 다른 부분들을 씌우거나(wrap) 감싸서(enclose) 다른 형식으로 보이게하거나 특정한 방식으로 동작하도록 하는 일련의 요소(elements)로 이루어져 있다.
  
 * tags로 감싸는 것으로 단어나 이미지를 다른 어딘가로 하이퍼링크(hyperlink)하거나 단어들을 이탤릭체로 표시하고 글씨체를 크게 또는 작게 만드는 등의 일을 할 수 있다. 

마크업 언어란?
마크업 언어는 태그 등을 이용하여 문서나 데이터의 구조를 명기하는 언어의 한 가지이다.
태그는 문서의 구조를 표현하는 역할을 하는데 이러한 태그 방법의 체계를 마크업 언어라 한다.
일반적으로 데이터를 기술하는 정도로만 사용되기에 프로그래밍 언어와는 구별된다. 다만 MXML이나 XAML처럼 특정 프로그래밍 언어와 강하게 연관되어 기능하거나 제한적으로 프로그래밍 언어의 기능을 갖춘 것도 일부 있는데 이 경우는 구변이 명확하지 않다.
마크업 언어는 표현적 마크업/절차적 마크업/기술적 마크업으로 분류된다.

## HTML 요소

1. 분석
<img src="https://media.vlpt.us/images/ssoon_d/post/cc1721f8-f508-4c16-a70b-610c88baf7af/image.png" width=500>

> 1. 여는 태그(opening tag)
>   - 요소의 이름으로 구성
>   - 여닫는 꺾쇠괄호로 감싸진다
>   - 요소가 시작되는 곳, 또는 효과를 시작하는 곳임을 암시한다
> 2. 닫는 태그(closing tag)
>   - 여는 태그에 추가로 요소의 이름 앞에 전방향 슬래시가 포함
>   - 요소의 끝을 의미
> 3. 컨텐츠(content)
>   - 요소의 내용(content)
> 4. 요소(element)
>   - 요소는 여는 태그와 닫는 태그, 그리고 컨텐츠로 이루어진다

2. 속성
<img src="https://media.vlpt.us/images/ssoon_d/post/db47e4c7-d1ba-4904-bdc4-1110d03fb85e/image.png" width=500>

> - 실제 컨텐츠로 표시되길 원하지 않는 추가적인 정보를 담고 있다.
> - 속성이 가져야 하는 것
> * 요소 이름(요소가 하나 이상 속성을 이미 가지고 있다면 이전 속성)과 속성 사이에 공백
> * 속성 이름 뒤에는 등호(=)
> * 속성 값의 앞 뒤에 열고 닫는 인용부호(" 또는 ')

3. 요소 중첩

> - 요소를 다른 요소 안에 넣을 수 있다
> <pre><code> <p>내 고양이는 <strong>아주</strong> 고약해.</p> </code></pre>
> - 태그의 열고 닫는 순서를 지켜야한다
> * 여기서는 strong이 더 나중에 나왔기 때문에 p보다 먼저 닫아 주었다

4. 빈 요소

> - 내용이 없는 요소들이 존재(img, btn, input 등)
> <pre><code> <img src="images/firefox-icon.png" alt="My test image"> </code></pre>

4. HTML 문서 해부

> - 내용이 없는 요소들이 존재(img, btn, input 등)
> <pre><code> <!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My test page</title>
  </head>
  <body>
    <img src="images/firefox-icon.png" alt="My test image">
  </body>
</html> </code></pre>

각 요소들이 어떻게 전체 HTML 페이지를 구성하는지 살펴보자
1. <!DOCTYPE html>
  - HTML은 버전별로 지원하는 태그가 다르기 때문에 HTML 버전을 표시하는 선언(위의 경우는 tml5)
2. <html></html>
  - 페이지 전체 컨텐츠를 감싸는 요소
  - 루트(root)요소
3. <head></head>
  - 문서의 상단부
  - 브라우저 화면에 직접적으로 보이지 않으며, 숨은 데이터를 정의하는 태그들이 들어가는 부분, 즉 문서 메타데이터를 담는다. 정보로는 제목, 스크립트, 스타일시트 등이 있다.

4. <body></body>
  - 페이지의 본문부분
  - 브라우저에 직접적으로 표혀하고 싶은 모든 컨텐츠를 담는 부분이다.

5. <meta charset="utf-8">
  - 문서가 사용해야 할 문자 집합을 utf-8로 설정
  - 어떠한 문자 컨텐츠도 다룰 수 있다.

6. <title></title>
  - 페이지의 제목 설정
  - 페이지가 로드되는 브라우저의 탭에 이 제목이 표시된다.

## 이미지

<pre><code> <img src="images/firefox-icon.png" alt="My test image"> </code></pre>

  - src : 이미지의 파일 경로
  - alt : 대체 텍스트, 설명적인 문자(descriptive text)를 쓰는 것이 좋다
  
## 문자 나타내기
<h1>~<h6>의 여섯개의 제목을 가진다.
  - 숫자가 커질 수록 크기는 작아진다.
  
문단
  - <p> 요소는 문자의 문단을 포함하기 위한 것

목록
  - <ul> : 순서가 없는 목록
  - <ol> : 순서가 있는 목록, type과 start 등으로 설정 가능
  - <li> : 목록의 각 항목들을 나타낸다

## 연결
  <a>로 문장 안의 어떤 단어를 링크로 만들 수 있다.
    - <a hr
  
-----------

### :clipboard: [참조] Reference

- [Learn the basics](https://velog.io/@ssoon_d/1.-Learn-the-basics)
- [MDN - HTML 기본](https://developer.mozilla.org/ko/docs/Learn/Getting_started_with_the_web/HTML_%EA%B8%B0%EB%B3%B8)
