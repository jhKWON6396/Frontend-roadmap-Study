# Accessibility

:writing_hand: *write by JaeHwanKwon*

---------
## 접근성
- 가능한 **많은 사람이 웹 사이트를 사용**할 수 있도록 하는 방법
- 장애를 가진 사람, 모바일 장치를 사용하는 사람, 느린 네트워크 연결을 사용하는 사람등을 포함
- 웹사이트는 **모든 사용자들이 차별없이 접근**할 수 있어야 한다.
- 브라우저 호환성 테스트를 거쳐 접근성을 고려해야 한다.
- 접근성을 위해서는 **의미론적인 HTML 구조(sementic HTML)로 마크업**하는 것이 가장 중요하다.

## Sementic HTML의 장점
- 개발에 용이하다
- 모바일 사용이 더 편리해진다
  * 시멘틱 구조의 HTML은 용량이 줄어들고, 반응형을 더 쉽게 만들 수 있다.
- SEO(검색엔진최적화)에 적합하다.

## 접근성 고려사항
1. 크로스 브라우징이 가능하도록 한다.
> [티스토리 - 크로스 브라우징](https://okayoon.tistory.com/entry/%ED%81%AC%EB%A1%9C%EC%8A%A4-%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A7%95cross-browsing)을 참조

2. 모든 값은 따옴표(")로 묶어준다.
3. 단일 태그의 마무리는 항상 '/>'로 해준다. ```<br/>```
4. 캐릭터셋을 반드시 지정해준다.
```<meta charset="utf-8">```
5. 이미지 태그에는 alt를 반드시 지정한다.
```<img src="" alt="" />```
6. 색상은 RGB코드로 지정한다.
7. HTML 코드 들여쓰기를 한다.
8. 이미지의 파일명은 의도가 드러나도록 작성한다.
9. class 이름을 지울 때, 상위 태그 box를 포함하여 지정한다.
 >  가장 큰 단위의 요소인 div 태그의 클래스 명은 wrap으로 통일하는 편이 좋음
10. 제목```<h>```태그를 적절하게 사용한다.
11. 사이즈는 px(픽셀) 단위를 주로 사용한다.
12. 표 형식을 나타낼 때에는 가급적 table 태그를 사용한다.
> Sementic HTML



-----------

### :clipboard: [참조] Reference

[MDN - What is accessibility?](https://developer.mozilla.org/ko/docs/Learn/%EC%A0%91%EA%B7%BC%EC%84%B1/What_is_accessibility) <br>
[MDN - HTML: 접근성을 위한 기초](https://developer.mozilla.org/ko/docs/Learn/%EC%A0%91%EA%B7%BC%EC%84%B1/HTML) <br>
[웹접근성을 고려한 HTML 코딩 작업시 규칙 또는 권장사항](https://penguingoon.tistory.com/162) <br>
[SoonJoo Gwon(권순주) - Accessibility](https://velog.io/@ssoon_d/5.-Accessibility)
