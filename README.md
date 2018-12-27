# 처음 시작하는 HTML & CSS
## 개발환경 설정
### 웹 브라우저
 * 크롬 [다운로드](https://www.google.co.kr/chrome/index.html)  
 * 파이어폭스 [다운로드](https://www.mozilla.org/ko/firefox/new/)  
 ### 웹브라우저 확장 프로그램
 * Web Developer
 * headingsmap
 * openWAX
 ----------------------------------------------------------------
 ### 에디터 및 확장프로그램
* Visual Studio Code [다운로드](https://code.visualstudio.com/)  
* Live Server
* Prettier-Code Formatter
* Auto Close Tag
* Auto Rename Tag
* vscode-icons
* Monokai-Contrast Theme
* Markdown Preview Enhanced
-----------------------------------------------------------------
### Git, Github
* Git [다운로드](https://git-scm.com/downloads)  
* Github [가입](https://github.com/)  
* 누구나 쉽게 이해할 수 있는 [Git입문](https://backlog.com/git-tutorial/kr/)  
-----------------------------------------------------------------
### 웹표준과 웹접근성  
웹표준이란  
웹에서 사용되는 표준적인 기술을 의미하며 구조 설계를 위한 HTML, 디자인 및 표현을 위한 CSS, 제어 및 동작을 위한 Javascript가 있다.  

웹접근성이란  
장애와 비장애에 구애받지 않고 누구나 접근할 수 있도록 하는 개념을 의미한다.  


-----------------------------------------------------------------
### HTML 명령어
#### HTML 기본 구조
```HTML
<!doctype html>
<HTML lang="ko-KR">
  <head>
    <title>처음 시작하는 HTML과 CSS</title>
  </head>
  <body>
    
  </body>
</HTML>

```
### 코드 사용할 때
 * ctrl + shift + d : 같은내용을 아랫줄에 복사하고 싶을 때
 * ctrl + 방향키 : 위아래 줄을 바꾸고 싶을 떄

-----------------------------------------------------------------
#### anchor
```HTML
<!DOCTYPE html>
<html lang="ko-KR">
<head>
  <meta charset="UTF-8">
  <title>하이퍼링크</title>
</head>
<body>
  <h1>하이퍼링크</h1>
  <p>처음 시작하는 HTML&CSS 과정은 <a href="http://www.multicampus.com/" target="_blank" title="새창">멀티 캠퍼스</a>에서 수강하실 수 있습니다.</p>
  <ul>
    <li><a href="./text.html">텍스트 관련 요소</a></li>
    <li><a href="./list.html">목록 관련 요소</a></li>
    <li><a href="#mark">문서 내에서 이동</a></li>
  </ul>
  <br><br><br><br><br><br><br><br><br><br>
  <br><br><br><br><br><br><br><br><br><br>
  <br><br><br><br><br><br><br><br><br><br>
  <br><br><br><br><br><br><br><br><br><br>
  <br><br><br><br><br><br><br><br><br><br>
  <h2>문서 내에서 이동하기</h2>
  <p id = 'mark'>하단 단락입니다.</p>
  <br><br><br><br><br><br><br><br><br><br>
  <br><br><br><br><br><br><br><br><br><br>
  <br><br><br><br><br><br><br><br><br><br>
  <br><br><br><br><br><br><br><br><br><br>
  <br><br><br><br><br><br><br><br><br><br>
</body>
</html>
```
-----------------------------------------------------------------
#### IMAGE
```HTML
<!DOCTYPE html>
<html lang="ko-KR">
<head>
  <meta charset="UTF-8">
  <title>이미지 삽입하기</title>
</head>
<body>
  <h1>콘텐츠 이미지</h1>
  <p> <img src="https://i.pinimg.com/474x/32/b8/79/32b879208349ec985f57676f8895189a.jpg" alt="" width="300" height="450"></p>
  <p> <img src="./asset/snowman.png" alt="눈내리는 풍경과 눈사람"width="450" height="300"></p>
  <p>
    <a href="http://www.multicampus.com">
      <img src="http://el.multicampus.com/landing/images/2016/common/logo.gif" alt="멀티캠퍼스">
    </a>
  </p>
</body>
</html>
```
-----------------------------------------------------------------
#### TEXT
```HTML
<!DOCTYPE html>
<html lang="ko-KR">
<head>
  <meta charset="UTF-8">
  <titl>텍스트 관련 요소</titl>
</head>
<body>
 <h1 class="brand">Web Cafe</h1>
 <hr>
 <p class="note">내용 입니다.</p>
 <p>달은 <strong>지구</strong>의 &yen; &euro; 주위를 돈다.</p>
 <p>지구는<br>떨어지는 우주의 먼지로 인해<br>매일 백 톤씩 무거워진다.</p>
  <p> <ABBR title = "Hyper Text Markup Language"> 	HTML </ABBR></p>
  <p>어제 <abbr title = "문화센터">문센</abbr>에 다녀왔다.</p>
 
</body>
</html>
```
-----------------------------------------------------------------
#### TABLE
* caption을 넣고, th와 td를 구분하자
```HTML
<!DOCTYPE html>
<html lang="ko-KR">
<head>
  <meta charset="UTF-8">
  <title>테이블 요소</title>
</head>
<body>
  <h1>테이블 예제(병합)</h1>
  <table>
    <caption>방송국 별 프로그램 방영시간표</caption>
    <tr>
      <th>&nbsp;</th>
      <th scope="col">ABC</th>
      <th scope="col">BBC</th>
      <th scope="col">CNN</th>
    </tr>
    <tr>
    <th scope="row">6pm-7pm</th>
    <td rowspan="2">영화</td>
    <td colspan="2">코미디</td>
    </tr>
    <tr>
      <th scope="row">7pm-8pm</th>
      <td>스포츠</td>
      <td>시사</td>
    </tr>

  </table>
</body>
</html>
```
-----------------------------------------------------------------
#### 
 * fieldset과 legend, lable은 한 set이다
 * input의 id(유닉한 이름값) 속성값을 lable의 for 속성값으로 넣어서 짝꿍을 만들어 준다.
 * 네이밍 방법  
  ** userName :CC(낙타케이스)  
  ** user_name :SC(뱀케이스)  
  ** user-name :CC(케밥케이스)  
 * POST VS GET  
  ** POST: 값을 던지기만 할거다.
```HTML
<!DOCTYPE html>
<html lang="ko-KR">
<head>
  <meta charset="UTF-8">
  <title>폼관련 요소</title>
</head>
<body>
<h1>Sign in to Github</h1>
<form action="https://formspree.io/skdisk6779@naver.com" method="POST">
  <fieldset>
    <legend>로그인 폼</legend>
    <label for="user-email">이메일 주소</label>
    <input type="email" id="user-email" required>
    <label for="user-pw">비밀번호</label>
    <input type="password" id="user-pw" required>
    <button type="submit">로그인</button>
  </fieldset>

</form>
</body>
</html>
```
-----------------------------------------------------------------
#### video
```HTML
<!DOCTYPE html>
<html lang="ko-KR">
<head>
  <meta charset="UTF-8">
  <title>비디오 삽입하기</title>
</head>
<body>
  <h1>HTML5 비디오 요소</h1>
  <video controls muted poster="./asset/snowman.png">
    <source src="./asset/Google-Developer-Stories.mp4">
    <track src="./asset/google-developer-stories-subtitles-en.vtt" kind="captions" srclang="en" label="English Caption">
  </video>
</body>
</html>
```
-----------------------------------------------------------------
#### iframe
```HTML
<!DOCTYPE html>
<html lang="ko-KR">
<head>
  <meta charset="UTF-8">
  <title>iframe 활용</title>
</head>
<body>
  <h1>iframe을 이용한 HTML 파일 삽입</h1>
  <!--실습 파일을 iframe으로 실습하기-->
  <iframe src="./anchor.html" width="400" height="300" frameborder="0"></iframe>




  <h1>iframe을 활용한 동영상 삽입</h1>
  <iframe width="400" height="300" src="https://www.youtube.com/embed/tmazLWAeGqk" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  <h1>iframe을 활용한 지도 삽입</h1>
  <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3433.155388614002!2d127.03807267027999!3d37.50173571008064!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x357ca3ff67128961%3A0x55a56e8ffc5bc5d!2z66mA7Yuw7Lqg7Y287IqkIOq1kOycoeyEvO2EsCjrqYDti7DsiqTtgJjslrQp!5e1!3m2!1sko!2skr!4v1545888904852" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
  <!-- * Daum 지도 - 지도퍼가기 -->
<!-- 1. 지도 노드 -->
<div id="daumRoughmapContainer1545888707784" class="root_daum_roughmap root_daum_roughmap_landing"></div>

<!--
	2. 설치 스크립트
	* 지도 퍼가기 서비스를 2개 이상 넣을 경우, 설치 스크립트는 하나만 삽입합니다.
-->
<script charset="UTF-8" class="daum_roughmap_loader_script" src="http://dmaps.daum.net/map_js_init/roughmapLoader.js"></script>

<!-- 3. 실행 스크립트 -->
<script charset="UTF-8">
	new daum.roughmap.Lander({
		"timestamp" : "1545888707784",
		"key" : "riwo",
		"mapWidth" : "600",
		"mapHeight" : "300"
	}).render();
</script>
</body>
</html>
```
-----------------------------------------------------------------
