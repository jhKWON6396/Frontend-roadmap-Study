# Writing Semantic HTML

:writing_hand: *write by JaeHwanKwon*

---------
## Semantic HTML
**문서의 의미에 맞게, 어플리케이션의 의미에 맞게 HTML을 작성하는 것을 의미**
즉, 각 요소의 의미에 맞게 HTML을 작성해야 하는 것

## 의미론적 태그(Semantic Element)

<img src="https://media.vlpt.us/images/ssoon_d/post/e15dbb49-af86-4be4-a16c-ba0ea8ba01ea/image.png" width=500>

1. ```<article>```
- 관심사에 따라 글을 작성하기 위해 사용하는 요소
- article 태그 내용이 독립적으로 존재해도 되는 경우에 쓰임
- 반드시 ```<h1>```~```<h6>```태그를 가져야 함
- article안에 section이 있어도 되고 그 반대로도 사용이 가능하다

2. ```<aside>```
- 본문 전체 내용과 직접적인 연관성이 없는 분리된 내용을 담을 때 사용
- 주로 사이드바나 배너광고, 위젯 등으로 이용된다

3. ```<details>```
- 추가적인 정보를 나타내거나 사용자가 요청하는 정보를 나타냄

4. ```<figure>```
- 일러스트, 다이어그램, 사진, 코드 등에 주석을 다는 용도로 사용

5. ```<footer>```
- 문서의 footer를 나타낼 때 사용
- 주소나 연락처, 저작권 등을 넣음
- 문서 내에서 한번만 사용되지만, 분리되어 있는 section이나 article의 해당 영역에 대한 footer로 사용할 수 있음

6. ```<header>```
- 문서의 header를 나타낼 때 사용
- 사이드 로코, 글로벌 링크, 소개 등을 넣음

7. ```<main>```
- 해당 페이지의 main 콘텐츠를 나타낸다
- 한 페이지에서 한번만 사용 가능

8. ```<mark>```
- 하나의 문서 내에서 다른 문맥과의 관련성을 나타내기 위해서 참조 목적으로 마킹되거나 하이라이트된 텍스트로 표현함

9. ```<nav>```
- 문서의 navigation을 나타낼 때 사용
- 보통 메뉴 영역으로 사용
- 브라우저가 네비게이션 영역을 알 수 있게되면, 검색엔진 색인에 도움을 줄 수 있음

10. ```<section>```
- 관심사 그룹에 따라 구획을 구분하기 위해 사용하는 요소
- 문법상 반드시 ```<h1>```~```<h2>```태그를 가져야 함
- 섹션의 관심사가 무엇인지 검색로봇에 알려준다

11. ```<time>```
- 24시간에서의 시간 혹은 그레고리력에서의 정밀한 날짜를 나타낸다


-----------

### :clipboard: [참조] Reference

[포림프 노트 - Semantic HTML(의미론적인 HTML)](https://porimp.tistory.com/entry/Semantic-HTML%EC%9D%98%EB%AF%B8%EB%A1%A0%EC%A0%81%EC%9D%B8-HTML) <br>
[생활코딩 - 의미론적 태그](https://opentutorials.org/module/1892/10954) <br>
[SoonJoo Gwon(권순주) - Writing semantic](https://velog.io/@ssoon_d/4.-Writing-Semantic-HTML)
