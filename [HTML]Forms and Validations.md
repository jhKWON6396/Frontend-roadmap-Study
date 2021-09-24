# Forms and Validations

:writing_hand: *write by JaeHwanKwon*

---------
## HTML 폼
- 사용자와 웹사이트 또는 어플리케이션이 **서로 상호 작용**하는 것 중 중요한 기술 중 하나
- 폼은 사용자가 **웹사이트에 데이터를 전송하는 것을 허용**한다.
- HTML 폼은 하나 이상의 **위젯**으로 만들어진다.
  * 셀렉 박스
  * 버튼
  * 체크박스
  * 라디오 버튼
  * 텍스트 필드
- 위젯들은 위젯을 설명하는 라벨과 함께 사용된다.

## 폼의 이해
- 폼은 입력된 데이터를 한 번에 서버로 전송한다
- 전송한 데이터는 웹 서버가 처리하고, 결과에 따른 또 다른 웹 페이지를 보여준다

## 폼 태그 동작방법
<img src="https://media.vlpt.us/images/ssoon_d/post/bb42ad1a-4666-4bc2-9721-7161f32b0291/image.png" width=500>

1. 폼이 있는 웹페이지를 방문
2. 폼 내용을 입력
3. 폼 안에 있는 모든 데이터를 웹 서버로 보낸다.
4. 웹 서버는 받은 폼 데이터를 처리하기 위해 웹 프로그램으로 넘김
5. 웹 프로그램은 폼 데이터를 처리
6. 처리결과에 따른 새로운 HTML 페이지를 웹 서버에 보낸다.
7. 웹 서버는 받은 HTML 페이지를 브라우저에 보낸다.
8. 브라우저는 받은 HTML 페이지를 보여준다.

##  폼 태그 속성
폼 속성은 보낼 위치와 보낼 방법을 결정한다.
- action
  * 폼을 전송할 서버 쪽 스크립트 파일을 지정
  * 해당 링크로 폼안에 있는 정보를 다른 페이지로 모두 넘어가게 한다.
  * 따로 링크를 지정하지 않으려면 #을 사용
- name
  * 폼을 식별하기 위한 이름을 지정
- accept-charset
  * 폼 전송에 사용할 문자 인코딩을 지정
- target
  * action에서 지정한 스크립트 파일을 현재 창이 아닌 다른 위치에 열도록 지정
    + _self : 기본 값, 현재 창에서 열림
    + _blank : 새창 혹은 새탭에서 열림
- method
  * 폼을 서버에 전송할 http 메소드를 지정 (GET 또는 POST)

<img src="https://media.vlpt.us/images/ssoon_d/post/1267d9ad-9603-4933-878a-7111ec709583/image.png" width=500>

  * GET
    + URL 끝에 데이터를 붙여 보낸다.
    + 보안에 취약
    + 지정된 리소스에서 데이터를 요청하는 경우인 요청파트에서 사용하는 메소드
  * POST
    + 내부적으로 보이지 않는다.
    + 데이터가 개인정보나 보안이 필요한 경우
    + 지정된 리소스에서 데이터를 처리할 경우인 쓰기, 수정, 삭제할 때 사용

## 폼을 구성하는 다양한 엘리먼트
1. 폼 엘리먼트 그룹 ```<field>,<legend>```
  ```<fieldset>``` 태그는 폼 태그 안에 관련 있는 폼 엘리먼트들을 그룹화 할 때 사용한다
  ```<fieldset>``` 태그 하위에 ```<legend>``` 태그를 사용하여 그룹화한 폼 엘리먼트들을 목적에 맞게 이름을 지정한다
    <fieldset style = "width:180px">
      <legend> fieldset과 legend</legend>
    </fieldset>
    
2. 다양한 모양을 가진 ```<input>```
사용자가 다양하게 폼 태그에 입력할 수 있는 공간을 만들어 준다.
- type
  * 태그 모양을 다양하게 변경할 수 있다.
  * text, radio, checkbox, password, button, hidden, fieupload, submit, reset 등
- name
  * 태그 이름을 지정
- readonly
  * 태그를 읽기전용으로 한다
- maxlength
  * 해당 태그 최대 글자 수를 지정
- required
  * 해당 태그가 **필수태그**로 지정된다
  * 필수 태그를 입력하지 않고 submit 버튼을 누르면 에러메시지가 웹 브라우저로 출력
- autofocus
  * 웹 페이지가 로딩되자마자 이 속성을 지정한 태그로 포커스가 이동
- placeholder
  * 태그에 입력할 값에 대한 힌트를 제공
- pattern
  * 정규 표현식을 사용하여 특정범위 내의 유효한 값을 입력받을 때 사용

3. 목록태그 ```<select>,<optgroup>,<option>```
```<select> -> <optgroup> -> <option>```
- ```<select>``` : 항목을 선택할 수 있는 태그
  * size : 한번에 표시할 수 있는 항목 수
  * multiple : 다중선택을 허용할 것인지를 지정
- ```<optgroup>``` : ```<select>```의 하위 태그
  * 목록들을 **그룹화**할 경우 사용한다
  * **label 속성**을 사용하여 그룹 이름을 지정
- ```<option>``` : ```<optgroup>```의 하위 태그
  * **목록**을 나타내는 

4. 여러 줄 글상자 ```<textarea>```
**여러 줄을 입력**받는 태그
  - row
    * 줄 크기 지정
  - cols
    * 한 줄에 입력될 크기 지정
  - placeholer
    * 텍스트 공간에 어떤 내용을 입력하면 되는지 알려줌

## HTML5 에서 추가된 요소

1. 입력 값 후보 ```<datalist>```
텍스트 상자에 **입력 값 후보 목록**을 지정할 경우 사용
> ```<input>```태그 속성 값으로 list를 지정하여 텍스트 박스 아래 그룹리스트로 출력

2. ```<input>``` 태그의 date
- **날짜**를 입력받기 위한 속성 값
- 날짜 선택을 위한 **달력**도 함께 표시된다.
- 이 값이 서버 프로그램에 전달되면 **자바 date 객체에 바로 데이터가 전달**된다
- 쉽게 date 데이터를 서버 프로그램에서 받을 수 있는 장점이 있다
> date 말고 month, week, time, datetime, datetime-local 추가

3. ```<input>``` 태그의 number와 range
**숫자를 입력**할 때 사용
- range
  * 슬라이더 형태로 UI로 렌더링
  * min, max 속성을 사용하여 최소 최댓값을 지정

4. ```<input>``` 태그의 color
**색상**을 입력받을 때 사용

## 웹표준 유효성 검사
- 웹 사이트가 W3C에서 지정한 웹표준을 얼마나 지켰는지 체크하고 수정하기위한 검사
- 간단한 방법으로 어느정도 표준이 지켜졌으며 어떤 오류가 발생하고 또 어떤 해결방안이 있는지를 알려주는 검사

## 검사 방법
**W3C 웹표준 유효성 검사도구**를 사용
다음과 같이 3개의 검사방법이 있다
<img src="https://media.vlpt.us/images/ssoon_d/post/adcd655c-3649-4abe-94e1-161215d8d4ea/image.png" width=500>

**1. Validate by URL** : 웹페이지의 URL을 입력하면 해당 경로의 페이지를 검사<br>
**2. Validate by File Upload** : 로컬상의 HTML파일을 업로드하여 유효성 검사<br>
**3. Validate by Direct Input** : 직접 HTML 코드를 Input text 창에 입력해 유효성 검사

## 검사를 하는 이유

- 웹표준이 잘 되어있는지 여부를 확인
  * 현재 사이트에서 웹표준이 맞지 않는 부분을 검출
  * 웹표준을 높이는데 도움
- 웹표준 유효성 인증마크를 부착할 수 있다.
  * 웹표준 검사결과가 완벽하다면 인증마크를 부착할 수 있다.
  * 홈페이지가 웹표준을 준수했다는 것을 가시적으로 나타낼 수 있다.



-----------

### :clipboard: [참조] Reference

[MDN - 나의 첫 HTML 폼](https://developer.mozilla.org/ko/docs/Learn/HTML/Forms/Your_first_HTML_form)
[Nextree - HTML : 폼(form) 이해](http://www.nextree.co.kr/p8428/)
[HTML 정보보내기 form태그_속성](https://m.blog.naver.com/PostView.nhn?blogId=govlrhaehfdl&logNo=221231502012&proxyReferer=https:%2F%2Fwww.google.com%2F)
[오마이사이트 - 웹표준 유효성 검사로 웹사이트 표준여부 검사하기](https://ohmysite.co.kr/web_common_sense.html?article_num=34&OTSKIN=layout_ptr.php&PB_1429088248=8&PB_1491885899=8)
[Forms and Validations](https://velog.io/@ssoon_d/2.-Forms-and-Validations)
