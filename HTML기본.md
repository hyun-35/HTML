# 1. HTML5 기본 용어

1. 태그와 요소 

   - 요소 : HTML 페이지를 구성하는 각 부품(제목, 본문, 이미지 등)

   - 태그 : 요소를 만들때 사용하는 작성 방법

     ```html
     <h5>Hello HTML5</h5>
     <p>즐거운 웹 프로그래밍 입문</p>
     ```

     <h5>Hello HTML5</h5>
     <p>즐거운 웹 프로그래밍 입문</p>

     

   - 속성 : 태그에 추가 정보를 부여할때 사용 하는 것

     ```html
     <h5 title='header'>Hello HTML5</h5> 
        속성이름	속성값
     ```

     <h5 title='header'>Hello HTML5</h5>

     

   - 주석 : 코드 설명 기록. <!-- 주석 -->





# 2. HTML5 페이지 구조와 작성법

```html
<!DOCTYPE html>  <!-- 웹브러우저에 HTML5문서라는 것을 알림 -->
<html>           <!-- 모든 html 페이지의 기본요소, 이 내부에 태그 작성 -->
<head>           <!-- body태그에 필요한 스타일시트와 자바스크립트 제공-->
	<title>Hello HTML5</title>    <!-- 웹브라우저에 표시하는 제목 지정-->
</head>
<body>           <!-- 사용자에게 실제로 보이는 부분 작성-->

</body>
</html>
```

1. <html> 태그 

   - html 태그의 lang속성 : ex. <html lang = 'ko'>

     > ko :  한국어
     >
     > en : 영어
     >
     > ja : 일본어
     >
     > ru : 러시아어
     >
     > zh : 중국어
     >
     > de : 독일어

   - head 태그 내부에 넣을 수 있는 태그

     > meta : 웹페이지에 추가 정보 전달
     >
     > title : 페이지 제목 지정
     >
     > script : 웹 페이지에 스크팁트 추가
     >
     > link : 웹 페이지에서 다른 파일 추가
     >
     > style : 웹 페이지에 스타일시트 추가
     >
     > base : 웹 페이지의 기본 경로 지정

2.  HTML5 페이지의 실행 : ㅇㅇ.html 또는 ㅇㅇ.htm 형식으로 저장

   ​											→ 크롬 브라우저에 드래그



# 3. HTML5 기본 태그

1. 글자 태그

   - 제목 : h1, h2, h3, h4, h5, h6 (숫자가 커질수록 글자가 작아짐)

   - 본문  

     - p : 본문 문단 생성
     
     - br : 줄 바꿈
     
     - hr : 수평 줄 삽입

   - 앵커 태그 : 다른 웹 페이지나 웹 페이지 내부의 특정 위치로 이동

     - a : 하이퍼링크 생성
     
     - href : Hyper Reference 의미

     ```html
     <a href='http://hanbit.co.kr'>한빛미디어</a>
              이동한 웹 페이지
     ```

   - 글자 모양 태그

     - b : 굵은 글자
     
     - i : 기울어진 글자
     
     - small :작은 글자
     
     - sub : 아래 첨자
     
     - sup : 위 첨자
     
     - ins : 밑줄 글자
     
     - del : 취소선이 그어진 글자

     ```html
     <i>
     	<h4>웹 표준 위반</h4>
     	<p>웹 표준 위반</p>
     </i>
     ```



2. 목록 태그

   - 내비게이션 태그 : 웹 사이트의 다른 웹 페이지로 이동할 수 있는 버튼

     - ul : 순서가 없는 목록 생성
     
     - ol : 순서가 있는 목록 생성
     
     - li : 목록 요소 생성

     ex. 기본 목록 만들기

     ```html
     <body>
         <ul>
             <!-- 첫번째 목록-->
             <li>
             	<b>과일</b>
             	<ol>
                     <li>사과</li>
     				<li>바나나</li>
     				<li>오렌지</li>
                 </ol>
             </li>
             <!-- 두번째 목록-->
             <li>
             	<b>채소</b>
             	<ol>
                     <li>상추</li>
     				<li>치커리</li>
     				<li>양배추</li>
                 </ol>
             </li>
         </ul>
     </body>	
     ```

     <ul>
             <!-- 첫번째 목록-->
             <li>
             	<b>과일</b>
             	<ol>
                     <li>사과</li>
     				<li>바나나</li>
     				<li>오렌지</li>
                 </ol>
             </li>
             <!-- 두번째 목록-->
             <li>
             	<b>채소</b>
             	<ol>
                     <li>상추</li>
     				<li>치커리</li>
     				<li>양배추</li>
                 </ol>
             </li>
         </ul>

3. 테이블 태그

   - table : 표 삽입

   ​            + 속성 : border - 표의 테두리 지정

   - tr : 표에 행 삽입

   - th : 표에 제목 셀 생성

   - td : 표의 일반 셀 생성

     > 속성(th, td 공통)  : colspan - 셀의 너비 지정
     >
     > ​                                rowspan - 셀의 높이 지정

   ex.  테이블 생성

   ```html
   <body>
       <table border='1'>
           <thead>
           	<tr>
               	<th></th>
                   <th>월</th>
                   <th>화</th>
                   <th>수</th>
                   <th>목</th>
                   <th>금</th>
               </tr>
           </thead>
           <tbody>
           	<tr>
               	<td>1교시</td>
               	<td>영어</td></td>
               	<td>국어</td>
               	<td>과학</td>
               	<td>미술</td>
               	<td>기술</td>
           	</tr>
       		<tr>
               	<td>2교시</td>
               	<td>도덕</td></td>
               	<td>체육</td>
               	<td>영어</td>
               	<td>수학</td>
               	<td>사회</td>
           	</tr>
       	</tbody>
       </table>
   </body>
   ```

   <table border='1'>
           <thead>
           	<tr>
               	<th></th>
                   <th>월</th>
                   <th>화</th>
                   <th>수</th>
                   <th>목</th>
                   <th>금</th>
               </tr>
           </thead>
           <tbody>
           	<tr>
               	<td>1교시</td>
               	<td>영어</td></td>
               	<td>국어</td>
               	<td>과학</td>
               	<td>미술</td>
               	<td>기술</td>
           	</tr>
       		<tr>
               	<td>2교시</td>
               	<td>도덕</td></td>
               	<td>체육</td>
               	<td>영어</td>
               	<td>수학</td>
               	<td>사회</td>
           	</tr>
       	</tbody>
       </table>
   


   ex. colspan , rowspan 속성 적용

   ```html
   <body>
       <table border="1">
           <tr>
               <th colspan="2">지역별 홍차</th>
           </tr>
           <tr>
               <th rowspan="3">중국</th>
               <td>정산소종</td>
           </tr>
           <tr><td>기문</td></tr>
           <tr><td>운남</td></tr>
           <tr>
               <th rowspan="4">인도 및 스리랑카</th>
               <td>아삼</td>
           </tr>
           <tr><td>실론</td></tr>
           <tr><td>다질링</td></tr>
           <tr><td>닐기리</td></tr>
       </table>
   </body>
   ```

   <table border="1">
           <tr>
               <th colspan="2">지역별 홍차</th>
           </tr>
           <tr>
               <th rowspan="3">중국</th>
               <td>정산소종</td>
           </tr>
           <tr><td>기문</td></tr>
           <tr><td>운남</td></tr>
           <tr>
               <th rowspan="4">인도 및 스리랑카</th>
               <td>아삼</td>
           </tr>
           <tr><td>실론</td></tr>
           <tr><td>다질링</td></tr>
           <tr><td>닐기리</td></tr>
       </table>



4. 미디어 태그

   - img 태그의 속성

     > src : 이미지의 경로 지정
     >
     > alt : 이미지가 없을때 나오는 글자 지정
     >
     > width : 이미지의 너비 지정
     >
     > height : 이미지의 높이 지정

   - audio, video 태그의 속성

     > src : 음악, 비디오 파일의 경로 지정
     >
     > preload : 음악, 비디오를 준비중일때 데이터를 모두 불러올지 여부 지정
     >
     > autoplay : 음악, 비디오의 자동 재생 여부 지정
     >
     > loop : 음악, 비디오의 반복 여부 지정
     >
     > controls : 음악, 비디오 재생 도구 출력 여부 지정
     >
     > width : 비디오의 너비 지정
     >
     > height: 비디오의 높이 지정

     ex. 이미지 삽입

     ```html
     <body>
         <img src="naver.png" alt="네이버" width="300" />
         <img src="Nothing" alt="그림이 존재하지 않습니다." width="300" />
     </body>
     ```

     ex. 음악 삽입

     ```html
     <body>
        <audio src="Kalimba.mp3" controls="controls"></audio>
     </body>
     ```

     ex. 웹 브라우저 제약이 없도록 음악 삽입 : source 태그 사용

     ​                                                                   → 웹 브라우저마다 지원한느 음악파일 확장자가 다른 문제 해결

     ```html
     <body>
         <audio controls="controls">
             <source src="Kalimba.mp3" type="audio/mp3" />
             <source src="Kalimba.ogg" type="audio/ogg" />
         </audio>
     </body>
     ```

     ex. 동영상 삽입

     ```html
     <body>
         <video width="640" controls="controls">
             <source src="Wildlife.mp4" type="video/mp4" />
             <source src="Wildlife.webm" type="video/webm" />
         </video>
     </body>
     ```

     ex. 동영상을 불러오는 동안 다른 이미지 보여주기

     ```html
     <body>
         <video width="640" controls="controls" poster="http://placehold.it/640x360">
             <source src="Wildlife.mp4" type="video/mp4" />
             <source src="Wildlife.webm" type="video/webm" />
         </video>
     </body>
     ```



5. 입력 양식 태그

   - form : 영역 생성 . method속성의 방식으로 action속성 장소에 데이터 전달

     > method : 전송방식 입력
     >
     > 				* get 방식 : 주소에 데이터를 입력해서 전달
     > 				* post 방식 : 주소 변겨 ㅇ없이 비밀스럽게 데이터 전달
     >
     > action : 전송위치 입력

   - input 

     > text : 글자 입력 양식 생성
     >
     > button : 버튼 생성
     >
     > checkbox : 체크 박스 생성
     >
     > file : 파일 입력 양식 생성
     >
     > hidden : 해당 표시 안함
     >
     > image : 이미지 형태 생성
     >
     > password : 비밀번호 입력 양식 생성
     >
     > radio : 라디오 버튼 생성
     >
     > reset : 초기화 버튼 생성
     >
     > submit : 제출 버튼 생성

   - textarea 

     > cols/rows : 여러 행의 글자 입력 양식 생성. cols는 너비를 지정하고 rows는 높이를 지정

   - select : 선택 양식 생성

     > multiple : 여러 항목 선택 가능 
     >
     > ​                  `<select multiple='multiple'>`

   - optgroup : 옵션 그룹화

   - option : 옵션 생성

   - fieldset : 입력 양식의 그룹 지정

   - legeng : 입력 양식 그룹의 이름 지정
   
   ex. 기본 입력 양식 태그
   
   ```html
   <body>
       <form>
           <!-- 사용자가 입력하는 입력 양식 -->
           <input type="text" name="text" value="text" /><br />
           <input type="password" name="password" value="password" /><br />
           <input type="file" name="file" value="file" /><br />
           <input type="checkbox" name="checkbox" value="checkbox" /><br />
           <input type="radio" name="radio" value="radio" /><br />
   
           <!-- 보이지 않는 입력 양식 -->
           <input type="hidden" name="hidden" value="hidden" /><br />
   
           <!-- 버튼 -->
           <input type="button" value="button" /><br />
           <input type="reset" value="reset" /><br />
           <input type="submit" value="submit" /><br />
           <input type="image" src="http://placehold.it/100x100" />
       </form>
   </body>
   ```

   ![캡처1](C:\Users\LSH\Desktop\캡처1.png)
   
   ex.  한 항목만 선택 : select 이용
   
   ```html
   <body>
       <select>
           <option>김밥</option>
           <option>떡볶이</option>
           <option>순대</option>
           <option>어묵</option>
       </select>
   </body>
   ```
   
   <select>
           <option>김밥</option>
           <option>떡볶이</option>
           <option>순대</option>
       	<option>어묵</option>
       </select>
   
   
   ex. 선택 옵션 묶기
   
   ```html
   <body>
       <select>
           <optgroup label="HTML5">
               <option>Multimedia Tag</option>
               <option>Connectivity</option>
               <option>Device Access</option>
           </optgroup>
           <optgroup label="CSS3">
               <option>Animation</option>
               <option>3D Transform</option>
           </optgroup>
       </select>
   </body>
   ```
   
   <select>
           <optgroup label="HTML5">
               <option>Multimedia Tag</option>
               <option>Connectivity</option>
               <option>Device Access</option>
           </optgroup>
           <optgroup label="CSS3">
               <option>Animation</option>
               <option>3D Transform</option>
           </optgroup>
       </select>
   
   
   
   ![캡처2](C:\Users\LSH\Desktop\캡처2.png)
   
   
   
   
   
   


   ​        

   


   ​        

   

   