# 처음 시작하는 HTML&CSS
## 개발환경 설정
### 웹브라우저
 * 크롬[다운로드](https://www.google.co.kr/chrome/index.html)
 * Firefox[다운로드](https://www.mozilla.org/ko/firefox/new/)
----------------------------
### 확장 프로그램
 * Web Developer
 * HeadingsMap
 * OpenWAX
 ------------------------
### 에디터 및 확장 프로그램
 * Visual Studio Code [다운로드](https://code.visualstudio.com/)
 * Live Server
 * Prettier-Code Formatter
 * Auto Close Tag
 * Auto Rename Tag
 * vscode-icons
 * Monokai-Contrast Theme
 * Markdown enhanced
------------------------------
### Git,Github
 * Git[다운로드](https://git-scm.com/downloads)
 * GitHub[가입하기](https://github.com/)
 * 누구나 쉽게 이해할수 있는 [Git입문](https://backlog.com/git-tutorial/kr/)
---------------------------
### 웹표준과 웹접근성  
웹표준이란  
웹에서 사용되는 표준적인 기술을 의미하며 구조 설계를 위한 HTML, 디자인 및 표현을 위한 CSS, 제어 및 동작을 위한 Javascript가 있다.  
  
웹접근성이란  
장애와 비 장애에 구애받지 않고 누구나 접근할 수 있도록 하는 개념을 의미한다.  
 
------------------------------
### HTML 명령어
#### HTML 기본구조
```html
<!doctype html>
<html lang="ko-KR">
  <head>
    <title>처음 시작하는 HTML과 CSS</title>
  </head>
  <body>

  </body>
</html>
```
### 텍스트 관련요소
**제목 요소**  
> h1,h2 등 제목의 의미를 가지는 컨텐츠를 마크업할때 사용할 수 있습니다.   
**단락 요소**  
> P 요소를 사용할 수 있으면 문단,혹은 단락의 의미를 가집니다.  
**축약어**  
> abbr 요소를 사용하여 마크업 합니다. 이때 abbr 요소는 줄임말 등 단축된 단어로 구성된 콘텐츠를 마크업 할 때 사용하며 title 속성을 사용하여 원래 의미를 표현할 수 있습니다.   

### 목록 관련 요소  
**비순서형 목록**  
> 목록형식의 콘텐츠 중에서 순서가 상관 없는 경우 사용할 수 있는 요소로 ul 요소를 사용할 수 있습니다. 이때 자식요소로는 li 요소만 올 수 있습니다.   
**순서형 목록**    
> 목록형식의 콘텐츠 중에서 순서가 중요한 경우 사용할 수 있는 요소로 ol 요소를 사용할 수 있습니다. 이때 자식요소로는 li 요소만 올 수 있습니다.   
**정의형 목록**    
> 용어 등을 정의할 때 사용하며 용어 제목은 dt 요소로 용어 설명은 dd 요소로 마크업 할 수 있으며 정의형 목록 영역임을 알 수 있도록 dl 태그를 상위에 사용합니다.   
### 하이퍼 링크 및 이미지 요소  
**하이퍼 링크**
> a 요소를 사용해서 마크업 합니다. 이때 a 요소 안에 텍스트나 이미지 등에 링크 기능을 부여할 때 사용할 수 있으며 링크의 목적지를 명시하고자 할때 href 속성에 연결하고자 하는 URL이나 file명을 지정합니다.   
**이미지**
> img 요소를 사용하고 src 속성에 이미지 파일의 URL이나 파일명을 지정합니다.
alt 속성의 경우 이미지 대체텍스트 역할입니다.
```html
<p><img src="./asset/snowman.png" alt="눈내리는 풍경과 눈사람" width="450"></p>
```
![멀티캠퍼스]
(http://el.multicampus.com/landing/images/2016/common/logo.gif)  

## CSS 스타일  
1. 상속  
2. 겹침  
3. 우선순위  
> CSS에서는 부모 요소에 지정한 스타일이 자식 요소에게 적용되는 현상을 상속이라고 부른다. 그러나 모든 속성이 상속되는 것은 아니다.   
> 겹침이란? 하나의 요소에 동일한 속성에 서로 다른 값이 적용되는 현상을 의미하며 기본적으로 구체성이 동일한 경우에는 가장 마지막에서 선언한 스타일이 우선적으로 적용됩니다.   
> 우선순위는 구체성에 따라 달라집니다. 이때 요소 선택자는 구체성 점수가 1점, 클래스 선택자는 구체성 점수가 10점, id 선택자는 구체성 점수가 100점 입니다.   

### 텍스트 관련 속성  
* font-family : 글꼴 지정  
* font-size : 글자 크기  
* font-weight : 글꼴 굵기  
* font-style : 글자의 기울임꼴  
* line-height: 단락 내에서 한줄의 높이를 지정  
* text-decoration : 밑줄 지정 및 삭제  
* text-shadow : CSS3 추가된 속성으로 글자의 그림자 지정  