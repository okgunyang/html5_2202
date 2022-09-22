#### 인터넷과 웹 환경의 발전

* 인터넷은 미 국방성이 군사정보의 공유를 목적으로 구축한 ARPANET에서 시작되었다.

* WWW(World Wide Web/W3)은 다양한 정보를 공유하기 위해 개발되었으며, '하이퍼텍스트'라는 개념을 채택하였다.

  + (하이퍼텍스트 : 연관된 여러 **데이터를 링크로 연결**해 사용자가 필요한 정보를 탐색할 수 있게 도와주는 정보탐색 구조.)

* HTML(HyperText Markup Language) : 웹을 위한 하이퍼텍스트 문서를 작성하는 언어.

* SGML(Standard Generalized Markup Language) 

  : 다양한 형식의 전자문서들의 구조와 내용을 기술하기 위해 제정된 국제표준.

* XML(eXtensible Markup Language) 

  :  SGML이 단순화된 부분집합으로 마크업 언어를 정의하기 위한 언어.

* 인터넷은 Client-Server Model을 기반으로한다.

  + Server : 제공하고자하는 정보들을 자신의 하드디스크에 보관하고 이를 외부에 공개해주는 컴퓨터.
  + Client : 서버에서 제공하는 정보를 받기 위한 컴퓨터.

* 인터넷에서는 데이터를 주고받기 위해 TCP/IP 통신 프로토콜을 적용한다.

  + TCP/IP 전송 프로토콜 : **인터넷에 연결되어 있는 시스템 사이**에 데이터를 송수신할 때 필요한 통신규약.

  + 통신 프로토콜 : 컴퓨터 사이에 정보를 전달하기 위해 필요한 규칙 및 약속의 집합.
  + TCP(Transmission Control Protocool) : 데이터의 흐름을 제어하고 데이터가 정확한지 확인하는 역할.  (패킷을 생성하고, 패킷이 제대로 전송되는지 확인한다.)
  + IP(Internet Protocool) : 데이터를 이동시킬 목적지를 정하는 역할.

* HTTP(HyperText Transfer Protocool) 서비스 프로토콜

  : **서버와 클라이언트 컴퓨터 사이**에 서비스를 위한 데이터 통신 규약.

* 각 호스트 컴퓨터는 하나의 IP주소와 도메인 이름을 가진다.

  + 도메인 이름 서버(Domain Name Server)에서 도메인 이름을 IP주소로 변환시켜준다.
  + 도메인 이름의 구조 : "호스트이름.소속기관.단체성격(.소속국가)" 3-4단계 형태.

* URL(Uniform Resource Locator)

  : 웹 문서를 통해 서버에서 자원의 위치를 표시하는 표준.

* 웹 브라우저

  : 웹 서버에 저장되어있는 하이퍼텍스트와 하이퍼미디어 정보를 사용자 기기의 화면에 보여주는 역할. 



#### HTML문서의 기본

+ <!DOCTYPE html> : 문서의 종류를 알리기 위한 선언

+ HTML문서의 요소는 내용과 이를 둘러싼 태그로 이루어져있다.

+ 태그의 이름에서 대소문자를 구분하지 않는다.

+ 단독태그 : <태그이름 /> - 시작 태그에서 태그이름 뒤에 /를 표시하면 종료태그를 작성하지 않아도 된다. ex) [br /] , [img /], [hr /]

+ 속성(Attribute) : 요소에 추가정보를 주기 위해서 사용한다. 각 속성은 빈칸으로 구분된다.

  <이름 = "속성값"> 의 형태로 작성된다. ex) [a href="ch02.html" target="blank"]

+ html문서는 head와 body요소로 구성되어 있다.

+ 특수문자 표기 시 &이름; 형식으로 표기한다.

  + 주요 특수 문자
    + 공백 문자 : & nbsp;
    + '<' : & lt;
    + '>' : & gt;
    + " : & quot;
    + & : & amp;

+ head 요소 

  + title 요소 - 제목을 적어놓는 요소.

  + meta 요소 - 문서 관리를 위한 메타정보를 나타내는 요소.

    : 문서 자체에 대한 정보나 키워드, 문자 인코딩 정보, 저자 정보 등

    ex) meta name="authors" content="이예지"

    ​     meta charset="utf-8"

+ 문자 인코딩 UTF-8과 EUC-KR

  + UTF-8(유니코드) : 현대 한글뿐 아니라 한글 고어, 각종 외국 언어의 문자 처리 가능.
  + ECU-KR(완성형코드) : 현대 한글 중 완성형 코드에 있는 문자만 표현 가능. UTF-8보다 표현할 수 있는 문자가 적다.

+ 설명문(Comment)

  : 소스코드 이외에 코드에 대한 설명, 정보를 기록할 때 사용한다. ''<!-- 설명 -->" 

+ 문서 내용을 표현하는 다양한 요소들

  + 제목(Headline) &lt;h1&gt;~&lt;h6&gt; 
  + 단락(Paragraph) &lt;p&gt;
  + 줄 바꿈(Link Break) &lt;br&gt;
  + 가로줄(Horizontal Line) &lt; hr&gt;
  + 작성된 형식 유지(Pre-formatted Text) &lt;pre&gt;
  + 단락 인용(Block Quotation) &lt;blockquote&gt;

+ 다양한 텍스트 표현들

  + <em>텍스트 강조(Emphasis)</em> &lt;em&gt;

  + <strong>강한 강조(Strong Emphasis)</strong> &lt;strong&gt;

  + <small>작은 글자</small> &lt;small&gt;

  + <mark>하이라이트(Marked) 효과</mark> &lt;mark&gt;

  + <sup>위 첨자(Superscript)<sup> &lt;sup&gt;

    <sub>아래 첨자(Subscript)<sub> &lt;sub&gt;

+ HTML5문서 규약에서는 가급적 문서의 출력 모양은 CSS를 사용하여 표현하는 것을 권장한다.

+ 목록 나열하기

  + 순서가 없는 목록(Unordered List) : &lt;ul&gt; 후 안에 &lt;li&gt; 요소 포함시켜야한다.

  + 순서가 있는 목록(Ordered List) : &lt;ol&gt; 후 안에 &lt;li&gt; 요소 포함시켜야한다.

  + 설명 목록(Description List 혹은 Definition List) : &lt;dl&gt;

    : &lt;dl&gt;요소 내에 설명하고자 하는 용어는 &lt;dt&gt;에 적고, 그 설명은 &lt;dd&gt;에 적어야한다.

+ 표 작성하기

  + &lt;table&gt;

    &lt;tr&gt;

     &lt;th&gt;제목&lt;/th&gt;

    &lt;/tr&gt;

    &lt;tr&gt;

    &lt;td&gt;내용&lt;/td&gt;

    &lt;/tr&gt;

    &lt;/table&gt;

+ 표의 구조적 표현

  + 셀 합치기

    + &lt;td rowspan="3"&gt; 아래 줄 3개의 셀을 합치겠다.
    + &lt;td colspan="3"> 옆 칸의 3개의 셀을 합치겠다.

  + 표를 설명하는 제목 입력 &lt;caption&gt;

  + 표의 머리줄, 몸체, 꼬리줄 표현 &lt;thead&gt;, &lt;tbody&gt;, &lt;tfoot&gt;

    : 표의 길이가 클 경우 머리줄과 꼬리줄을 고정한 채 몸체만 스크롤하는 것이 가능하다.

+ 웹문서 구조화 요소

  : 컴퓨터에게 문단에 대한 의미를 정확하게 지정해주기 위한 요소들로써, 화면상으로는 모양이 구분되어 표시되지 않는다.

  + 머리말 &lt;header&gt; : 웹 문서에서 페이지 혹은 섹션의 머리말 영역을 나타낼 때 사용.

  + 탐색 &lt;nav&gt; : 내비게이션 링크(<small>웹 문서의 한 지점에서 다른 웹문서나 문서 내의 다른 부분으로 이동하는 것.</small>)를 표현할 때 사용.

  + 독립된 본문 &lt;article&gt; : 하나의 신문안에 여러 개의 기사처럼 독립된 본문을 나타낼 때 사용. header, footer, section요소가 포함될 수 있음.

  + 문서내 섹션 그룹 &lt;section&gt; : 웹문서 내에서 절 단위로 구분하거나 의미가 비슷한 그룹으로 문서를 구분하여 묶기 위해서 사용.

  + 부수 정보 &lt;aside&gt; : 본문의 내용과 구별되는 별개의 정보를 표현하기 위해 사용.

  + 꼬리말 &lt;footer&gt; : 웹 문서에 꼬리말에 해당하는 저자 정보, 이용조건, 관련 링크 등을 나타내기 위해 사용.



#### 링크와 멀티미디어

1. 링크

+ 하이퍼텍스트(HyperText) : 서로 연관된 문서나 텍스트 조각들을 연결하여 원하는 정보를 찾아가도록 하는 것.

+ 하이퍼미디어(HyperMedia) : 텍스트뿐만 아니라 이미지, 그래픽, 비디오 등 멀티미디어 정보가 서로 연결되어 있는 것.

+ 노드 : HTML문서나 멀티미디어 정보를 표현하는 기본 단위.

+ 앵커(anchor)  : 노드에 해당하는 HTML문서 내에서 링크의 출발점이나 도착점.

+ &lt;a&gt;요소를 이용한 문서 간 이동.

  +  위치 지정 방법

    + 절대 속성 : http:// 로 시작하는 URL형식의 인터넷 주소 표기.

    + 상대 속성 : http://로 시작하지 않는 경우. 

      ​		현재 문서와 같은 폴더의 위치에서부터 표기된 주소로 이동.

  + ex) &lt;a href="파일이름 or URL주소" title="설명">
  + title 속성 : 하이퍼링크 위에 마우스를 가져가면 나오는 말풍선 속 설명.

+ &lt;a&gt;요소를 이용한 문서 내 특정 위치로 이동.

  + 이런한 기능의 링크를 사용하려면 목적지 앵커와 시작점 앵커를 설정해야 함.

  + &lt;a id="고유아이디"&gt; &lt;/a&gt; :  문서 내 이동할 목적지 설정.

    &lt;a href="#고유아이디"&gt; 시작점 - 링크가 설정된 '고유아이디'의 위치로 이동&lt;a&gt;

2. 이미지 사용하기

+ 이미지 파일 종류 : 웹 브라우저에서 공통적으로 사용할 수 있는 이미지 파일은 GIF, JPEG, PNG가 있음.

  +  GIF(Graphic Interchange Format) : JPEG, PNG보다 파일 크기가 작고, 자연스러운 장면을 표현하지 못함.
  + JPEG(Joint Photographic Experts Group) : 복잡한 그림, 사진 등 색상을 많이 사용하는 이미지에 적함.
  + PNG(Portable Network Graphic) : GIF와 JPEG 형식의 장점, 비압축 형식의 BMP형식의 장점도 고려함.
  + 사진과 같이 색상의 개수가 많은 이미지를 다룰 때는 JPEG 형식이 적합하고, 색상의 개수가 적거나 간단한 도형으로 이루어진 이미지를 다룰 때는 GIF가 압축률이 높음.

+ 이미지 삽입 

  + 사용할 이미지 파일을 HTML파일과 동일한 폴더 또는 하위 폴더에 저장해야함.

  + 이미지 파일이 HTML문서와 같은 폴더에 있지 않다면 src에 경로를 적어줘야함.

    ex) image파일 안에 이미지 파일이 있다면 src="image/파일이름" 의 형태로

  + ex) &lt;img src="파일이름" width="크기" height="크기" alt="대체 텍스트"&gt;

  + &lt;img&gt;요소의 alt(alternate text-대체 텍스트) 속성 

    : 이미지를 표시 못하는 경우에 대체 텍스트가 사용됨.

  + &lt;figure&gt; 요소

    + 그림, 사진, 다이어그램과 텍스트 등의 콘텐츠를 함께 묶어 하나의 독립된 단위로 취급하고 싶을 때 사용.
    + ex) &lt;figure&gt; &lt;img src="intro.jpg" alt="책표지이미지"&gt; &lt;/figure&gt;

  + &lt;figcaption&gt; 요소

    + &lt;figure&gt; 요소를 위한 제목을 표현하는 요소. figure내에 위치하면 됨.

  + &lt;figure&gt; 요소를 위한 제목을 표현하는 요소. &lt;figure&gt;내에 위치하면 됨.

+ 이미지에 하이퍼링크 연결

  + ex) &lt;a href="링크할 곳의 파일이름"&gt; &lt;img src="이미지 파일이름"&gt; &lt;/a&gt;

3. 오디오와 비디오

+ HTML5는 외부객체로 표현하지 않고 별도의 플러그인 설치없이 오디오와 비디오 재생 가능.

+ 오디오 삽입하기

  + &lt;audio controls autoplay src="재생할 사운드 파일 이름"&gt;

  + contorls 속성 : audio요소 내에 적을 시 미디어 제어기를 표시하겠다는 의미.

  + autoplay 속성 : 파일을 로드하자마자 자동으로 재생한다는 의미.

  + loop 속성 : 사운드를 반복 재생시킬 횟수를 지정.

  + 오디오 타입을 지원하지 않을 경우를 대비해서 &lt;audio&gt;요소 내의 &lt;source&gt;요소를 이용하여 같은 내용을 여러 형식으로 작성한 오디오 파일들을 지정할 수 있음.

     ex) &lt;audio controls autoplay&gt;

    &lt;source src="song.mp3" type="audio/mp3"&gt; 

    &lt;source src="song.mp3" type="audio/ogg"&gt; 	

    &lt;/audio&gt;

  + type 속성 : 오디오 파일의 MIME 형식을 지정.

    + MIME 형식 : 멀티미디어 파일에 대한 형식을 종류별로 구분하도록 한 표기.

      ex) "audio/mp3", "audio/ogg" 등

  + preload 속성 

    + auto : 웹 브라우저가 페이지를 로드하고 바로 오디오 파일 다운로드.
    + metadata : 사용자가 재생시키기 전까지는 메타데이터만 다운로드.
    + none : 사용자가 재생을 시작하기 전까지는 파일을 다운로드 하지 않음.

+ 비디오 삽입하기

  + &lt;video controls src="재생할 비디오 파일 이름" width="폭" height="높이"&gt;
  + src, controls, loop, autoplay 속성은 &lt;audio&gt; 요소의 속성들과 동일.
  + width, height 속성 : 비디오 콘텐츠가 표시될 영역의 크기를 설정. 비디오 자체의 크기와 일치하지 않을 경우 비디오 콘텐츠가 늘어나거나 잘릴 수 있음.
  + videoWidth, videoHeight : 비디오 자체의 너비, 높이를 반환하는 속성.
  + poster : 비디오가 로딩되고 있을 때 보여줄 이미지를 지정하는 속성.
  + preload : 브라우저가 미리 동영상을 로딩할지 지정하는 속성. (&lt;audio&gt;와 동일)
    + 속성이 metadata인 경우 비디오의 첫 프레임이 나타남.

4. 객체 포함하기 

+ HTML 문서에서는 다른 HTML파일이나 이미지, 멀티미디어 파일 등 외부 객체를 포함할 수 있음.
+ &lt;iframe&gt;  요소 : 새로운 브라우저로 이동하지 않고 한 화면에서 링크로 연결된 내용을 같이 볼 수 있음.
  + &lt;iframe&gt;의 속성
    + src : 파일의 url 지정.
    + width, height : 삽입될 브라우저 프레임의 가로와 높이의 크기 지정.
    + name : 브라우저 프레임의 이름 지정.
    + &lt;a&gt;요소의 target속성에 &lt;iframe&gt;의 이름을 지정하면 링크를 클릭할 때 연결된 문서가 내부 프레임에 나타남.
  + ex) &lt;iframe src="내부 프레임에 출력할 파일의 URL" width="폭" height="높이" name="이름"&gt; &lt;/iframe&gt;
+ &lt;embed&gt; 요소 
  + &lt;iframe&gt;와 마찬가지로 src, width, height의 속성을 가짐.
  + ex) &lt;embed src="삽입할 파일의 URL" width="폭" height="높이"&gt; 
+ HTML5는 XML과 호환되기 때문에 XML로 작성된 문서를 웹 페이지에 바로 포함시킬 수 있음.
  + &lt;canvas&gt;요소로 그림 그리기
  + &lt;svg&gt;요소로 벡트 그래픽스 그리기
  + &lt;math&gt;요소로 수학 공식 표현하기



#### html 기본 태그 정리

1. 제목 

   &lt;h1>글자&lt;/h1&gt; : h1 ~ h6까지 있음. 

   + 예시

     <h1>h1</h1>

     <h2>h2</h2>

     <h6>h6</h6>


2. 링크 

   &lt;a href = "URL"&gt; 깃허브주소로이동&lt;/a&gt;

   + 예시

     <a href="www.github">깃허브주소로이동</a> 


3. 강조

   &lt;em&gt;글자&lt;em&gt;

   + 예시

     <em>em태그</em>

   &lt;strong&gt;글자&lt;/strong&gt;

   + 예시

     <strong>strong태그</strong>


4. 가로 선

   &lt;hr&gt;

   + 예시

     <hr>


5. 단락 설정

   &lt;p&gt;문자열&lt;/p&gt;


6. 굵은 글꼴

   &lt;strong&gt;문자열&lt;/strong&gt;

   + 예시

   ​	<strong>b태그</strong>


7. 밑줄

   &lt;ins&gt;문자열&lt;/ins&gt;

   + 예시

     <ins>u태그</ins>

8. 개행

   &lt;br&gt;

9. 이미지

   &lt;img src="그림 파일명"&gt;

10. 목록

    + &lt;ul&gt; : 번호 부여 x

      &lt;li&gt; 1 &lt;/li&gt;

      &lt;li&gt; 2 /li&gt;

      &lt;/ul&gt;

      예시

      <ul>

      <li>1</li>

      <li>2</li>

      </ul>

    + &lt;ol&gt; : 번호 부여 o

      &lt;li&gt; 1 </li&gt;

      &lt;li&gt; 2 </li&gt;

      &lt;/ol&gt;

      예시

      <ol>

      <li>1</li>

      <li>2</li>

      </ol>


11. 특수 기호 (' '사이 공백 제거해야함)

    + '& amp;' : &amp;
    + '& lt;' : &lt;
    + '& gt;' : &gt;
    + '& quo;' : "
    + '& nbsp;' : 공백


12. 표 작성하기

    + 테이블 시작과 끝 태그 : &lt;table&gt; &lt;/table&gt;

    + 행 태그 tr(table row) : &lt;tr&gt; &lt;/tr&gt;

    + 셀 태그 td(table data) : &lt;td&gt;내용&lt;/td&gt;

    + 예시

      <table&gt;

       &lt;tr&gt; &lt;td&gt;1행1셀&lt;/td&gt; &lt;td&gt;1행2셀&lt;/td&gt;&lt;/tr&gt;

       &lt;tr&gt; &lt;td&gt;2행1셀&lt;/td&gt; &lt;td&gt;2행2셀&lt;/td&gt;&lt;/tr&gt;

       &lt;/table&gt;

      <table>

      <tr><td>1행1셀</td><td>1행1셀</td></tr>

      <tr><td>2행1셀</td><td>2행2셀</td></tr>

      </table>

    + 기타 기능

      + 표 테두리 굵기 

        예시 

        &lt;table border="1"&gt;

      + 표 크기

        예시

        &lt;table width="150"&gt;

      + 표의 셀 간격

        예시

        &lt;table cellspacing="10"&gt;

      + 표의 여백

        예시

        &lt;table cellpadding="10"&gt;

      + 표의 셀 병합

        예시

        &lt;td colspan="2"&gt; : 2개의 셀을 가로로 병합

        &lt;td rowspan="2"&gt; : 2개의 셀을 세로로 병합

      + 표 위의 제목

        예시

        &lt;table&gt; 

        &lt;caption&gt; 표 제목 &lt;caption&gt;

        &lt;table&gt;


13. 폼 요소 작성하기
    + form : 기본
        사용자로부터 정보(아이디, 비밀번호 등)를 입력받을 때 사용하는 태그
        &lt;form action="login.jsp" method="post"&gt;
            폼 컨트롤,...
        &lt;/form&gt;
            + action 속성 : 폼에 입력된 정보를 받는 곳
            + method 속성 : 폼에 입력된 정보를 전송하는 방식으로 get과 post가 있음

        + 컨트롤 그룹
        &lt;fieldset&gt;
            &lt;legend&gt;그룹명&lt;/legend&gt;
            폼 컨트롤,....
        &lt;/fieldset&gt;
        서로 관련성 있는 폼 컨트롤 요소를 묶어 줄 수 있으며, 열고 닫는 태그 사이에 원하는 폼 컨트롤 들을 입력하면 됨
        legend는 컨트롤 그룹의 이름을 표시할 수 있음


        + 문자(텍스트) 입력
        &lt;input type="text"&gt;
        사용자로부터 문자(= text)를 입력받는 태그로서 type 속성을 생략하면 text가 됨

        + 비밀번호 입력
        &lt;input type="password"&gt;
        사용자로부터 비밀번호를 입력받는 태그
        속성을 type="password"로 변경해주면 사용자가 입력하는 정보가 외부로 노출되지 않음

        + 숫자 입력
        &lt;input type="number"&gt;
        사용자로부터 숫자를 입력받는 태그
        min, max, step 속성을 지정할 수도 있음

        + 날짜 입력
        &lt;input type="date"&gt;
        사용자로부터 날짜를 입력받거나 달력을 표시할 수 있는 태그
        
        + 월 입력
        &lt;input type="month"&gt;
        사용자로부터 날짜 중에서 달력을 활용하여 년과 월을 입력할 수 있는 태그

        + 주 입력
        &lt;input type="week"&gt;
        사용자로부터 날짜 중에서 몇 번째 주인지를 입력할 수 있는 태그

        + 시간 입력
        &lt;input type="time"&gt;
        사용자로부터 시간을 입력할 수 있는 태그

        + 이메일 입력
        &lt;input type="email"&gt;
        사용자로부터 이메일을 입력 받을 수 있는 태그

        + 전화번호 입력
        &lt;input type="tel"&gt;
        사용자로부터 이메일을 입력 받을 수 있는 태그

        + 검색어 입력
        &lt;input type="search"&gt;
        사용자로부터 검색어를 입력 받을 수 있는 태그

        + 인터넷 주소 입력
        &lt;input type="url"&gt;
        사용자로부터 인터넷 주소인 URL을 입력 받는 태그

        + 범위값 입력
        &lt;input type="range"&gt;
        사용자로부터 슬라이더를 활용하여 범위에 해당하는 값을 입력 받을 수 있는 태그
        min, max, step 속성을 지정할 수도 있음

        + 체크박스
        &lt;input type="checkbox"&gt;
        사용자가 On/Off의 형태의 선택사항으로 값을 받고자 할 경우 사용하며, 사각형 모양
        checked 속성을 지정할 수 있음

        + 라디오 버튼
        &lt;input type="radio"&gt;
        사용자가 여러 가지 중에서 하나만 꼭 선택해야 하는 값을 받고자 할 경우 사용, 둥근 모양
        여러 개의 라디오 버튼에서 하나 만을 꼭 선택해야 하므로 반드시 name 속성이 같아야 함
        checked 속성을 지정할 수 있음

        + 컬러 선택 버튼
        &lt;input type="color"&gt;
        사용자가 컬러 팔레트를 활용하여 원하는 색상의 값을 입력할 수 있는 태그

        + 전송 버튼
        &lt;input type="summit"&gt;
        사용자가 폼에 입력한 정보를 action 속성에 입력한 곳으로 값을 전송할 수 있는 태그

        + 취소 버튼
        &lt;input type="reset"&gt;
        사용자가 입력한 내용을 소거하여 초기화하는 태그

        + 일반 버튼
        &lt;input type="button"&gt;
        사용자가 이 버튼을 눌렀을 경우 이벤트를 발생시키기 위한 태그

        + 이미지 버튼
        &lt;input type="image"&gt;
        버튼에 이미지를 추가할 수 있는 태그

        + 파일 첨부 버튼
        &lt;input type="file"&gt;
        파일을 첨부할 수 있도록 하는 태그
        accept 속성을 활용하여 특정 파일만 추가할 수 있도록 할 수 있음

        + 펼침 선택 상자
        &lt;select name="컨트롤이름"&gt;
            &lt;option value="전송될값"&gt;표시되는 텍스트&lt;option&gt;
            ,....
        &lt;/select&gt;
        클릭하면, 아래로 펼쳐져 늘어지는 목록상자가 표시되어 그 중에서 사용자가 값을 선택할 수 있도록 해주는 태그로서 부속요소로 option 요소를 활용해야 함
        처음 부터 특정 값을 선택되게 하려면, 해당 option 요소에 selected 속성을 추가함

        + 메모 상자
        &lt;textarea name="컨트롤이름" rows="행수" cols="한 줄당 글자수"&gt;
        &lt;/textarea&gt;
        여러 줄로 많은 내용의 텍스트를 입력받을 수 있는 태그

        + 폼 컨트롤들의 지정가능한 속성
        accept : file 컨트롤에 지정가능하며, 파일을 업로드 컨트롤에서 기대하는 파일 유형을 암시

        alt	: image 컨트롤에 지정가능하며, 이미지 유형에 대한 대체 속성. accessibiltiy 측면에서 필요.

        autocomplete : 모든 컨트롤에 지정가능하며,양식 자동생성 기능 (form autofill) 암시

        autofocus : 모든 컨트롤에 지정가능하며,	페이지가 로딩될때 양식 제어에 오토포커스되므로 하나의 컨트롤에만 지정해야 함

        capture	: file 컨트롤에 지정가능하며, 파일 업로드 제어에서 input 방식에서 미디어 capture

        checked	: radio, checkbox 컨트롤에만 지정가능하며, 커맨드나 컨트롤이 체크 되었는지의 여부를 지정, 라디오 버튼의 경우 한 그룹 내에서 하나의 컨트롤에만 적용해야함

        dirname	: text, search	컨트롤에 지정가능, 양식 전송시 요소의 방향성을 전송할 때 양식 필드의 Name

        disabled : 모든 컨트롤에 지정가능, 양식 컨트롤이 비활성화되었는지의 여부를 지정하며, 지정된 컨트롤은 값을 전송할 수 없음

        formaction : image, submit 컨트롤에 지정가능, 양식 전송시 URL 사용하기

        formenctype	: image, submit	컨트롤에 지정가능, 양식의 데이터 인코딩 유형이 양식 전송시 사용될 것

        formmethod : image, submit 컨트롤에 지정가능, 양식 전송시 HTTP 방식을 사용

        formnovalidate : image, submit 컨트롤에 지정가능, 양식 전송시 양식 컨트롤 확인을 무시하기

        formtarget : image, submit 컨트롤에 지정가능, 양식 전송시 브라우징 맥락

        height : image 컨트롤에만 지정가능, 이미지 높이에서 height 속성과 같음

        list : datalist 자동입력 옵션의 id 속성값

        max	: 숫자 타입 입력이 가능한 컨트롤에 지정가능, 최대값

        maxlength :	password, search, tel, text, url 컨트롤에 지정가능하며,	value의 최대 길이 (문자수)

        min	: 숫자 타입 입력이 가능한 컨트롤에 지정가능, 최소값

        minlength :	password, search, tel, text, url 컨트롤에 지정가능, value의 최소 길이 (문자수)

        multiple : email, file 컨트롤에 지정가능, 불리언값. 여러 값을 허용할지의 여부

        name : 모든 컨트롤에 지정가능, input 양식 컨트롤의 이름. 이름/값 짝(name/value pair)의 일부로서 양식과 함께 전송된다

        pattern : password, text, tel 컨트롤에 지정가능, value 가 유효하기 위해 일치해야 하는 패턴

        placeholder : password, search, tel, text, url 컨트롤에 지정가능, 양식 컨트롤이 비어있는 때 양식 컨트롤에 나타나는 내용

        readonly : 문자나 숫자로 입력하는 것은 모두 가능, 불리언값. 이 값은 수정이 불가능함

        required : 입력 또는 선택하는 컨트롤은 모두 가능하며, 양식이 전송되기 위해서 반드시 입력하거나 확인이 필요한 값

        size : email, password, tel, text 컨트롤에 지정가능, 컨트롤의 크기

        src	: image 컨트롤에 지정가능, 이미지 출처의 주소에서 src 와 같은 속성값

        step : 숫자 입력이 가능한 컨트롤에 지정가능, 유효한 증분적인 (Incremental)값

        type : input 컨트롤에 지정가능, 양식 컨트롤의 유형

        value :	모든 컨트롤에 지정가능, 이름/값 짝(name/value pair)의 일부로서 양식과 함께 전송된다
        
        width : image 컨트롤에 지정가능, 이미지의 width 속성과 같다    



# html5-tag cheat sheet

## 구성 요소
* **&lt;html&gt;** 문서의 루트요소, 모든 HTML요소 루트 요소내에 포함되어야 함
* **&lt;head&gt;** 문서의 메타데이터 집합요소, 문서 제목, style, javascript 요소 포함
* **&lt;body&gt;** 문서의 본문 요소

## 메타 요소
* **&lt;title&gt;** 문서의 제목으로 텍스트만 포함됨
* **&lt;meta&gt;** 다양한 문서 정보를 담음&lt;
* **&lt;style&gt;** css 문서에 직접 기술할 때
* **&lt;link&gt;** 문서에 외부문서를 연결
* **&lt;base&gt;** 문서의 상대 경로에 대한 기본 URL을 정의

## 스크립팅 요소
* **&lt;script&gt;** 문서에 자바스크립트 파일을 삽입하거나 코드를 기술할 때
* **&lt;noscript&gt;** 자바스크립트 지원하지 않을 경우, 대신 제공할 풀백 콘텐츠 정의

## 섹션 요소
* **&lt;section&gt;** 장이나 절 등으로 구성할 수 있는 콘텐츠 섹션을 정의할 때
* **&lt;nav&gt;** 문서의 주요 내비게이션을 정의할 때
* **&lt;article&gt;** RSS 피드로 재배포할 가치가 있는 독립된 콘텐츠를 정의할 때, 재배포여부 중요치 않음
* **&lt;aside&gt;** 본문 콘텐츠와 연관성이 적은 콘텐츠를 정의할 때
* **&lt;header&gt;** 페이지나 섹션 등의 헤더를 정의할 때
* **&lt;footer&gt;** 페이지나 섹션 등의 푸터를 정의할 때
* **&lt;address&gt;** 연락처 정보를 정의할 때
* **&lt;h1&gt; ~ &lt;h6&gt;** 콘텐츠 블록의 제목을 정의할 때

## 그룹 요소
* **&lt;div&gt;** 콘텐츠 블록의 시멘틱한 의미를 가지고 있지는 않지만, 디자인이나 개발 이슈로 인해 콘텐츠 블록을 그룹화하고자 할 때
* **&lt;main&gt;** 문서의 주요 콘텐츠 영역을 정의할 때, 문서에는 하나의 &lt;main&gt;만 존재
* **&lt;p&gt;** 단락 콘텐츠를 정의할 때
* **&lt;ul&gt;** 비순서형 목록을 마크업할 때
* **&lt;ol&gt;** 순서형 목록을 마크업할 때
* **&lt;li&gt;** 순서형 또는 비순서형 목록의 목록 항목을 정의할 때
* **&lt;dl&gt;** 정의형 목록을 마크업할 때
* **&lt;dt&gt;** 정의형 목록의 용어 제목
* **&lt;dd&gt;** 정의형 목록의 용어 설명
* **&lt;figure&gt;** 요소는 이미지, 오디오, 비디오, 표를 포함
* **&lt;figcaption&gt;** 요소에 포함된 콘텐츠에 대한 캡션을 정의할 때
* **&lt;blockquote&gt;** 인용 콘텐츠 블록을 정의할 때
* **&lt;pre&gt;** 공백이나 줄바꿈 등의 입력 형식 그대로 화면에 렌더링하고자 할 때
* **&lt;hr&gt;** 단락의 주제를 구분하고자 할 때		

## 텍스트 요소
* **&lt;a&gt;** 하이퍼링크를 지정할 때
* **&lt;em&gt;** 텍스트를 강조하고자할 때
* **&lt;strong&gt;** 특별히 중요한 콘텐츠의 의미를 부여하고자 할 때
* **&lt;i&gt;** 단순 이텔릭체 표현에서 분위기를 전환하려는 의미의 텍스트 나타냄. 전문용어, 관용구, 생각 또는 선박 이름 등에 사용
* **&lt;b&gt;** 텍스트를 볼드체로 표현
* **&lt;mark&gt;** 텍스트를 하이라이트로 지정하고자 할 때
* **&lt;small&gt;** 저작권 정보 등과 같이 작은 크기의 텍스트 콘텐츠에 사용
* **&lt;abbr&gt;** 축약어를 정의할 때
* **&lt;cite&gt;** 결과물의 인용 및 참조를 정의할 때
* **&lt;q&gt;** 인라인 인용구를 정의할 때
* **&lt;time&gt;** 기계적으로 이해하거나 처리할 수 있는 날짜 및 시간정보를 정의할 때
* **&lt;date&gt;** 기계적으로 이해하거나 처리할 수 있는 날짜 및 시간정보를 정의할 때
* **&lt;code&gt;** 소스 코드를 정의할 때
* **&lt;var&gt;** 프로그램에서의 변수, 식별자 등의 의미를 정의할 때
* **&lt;samp&gt;** 시스템의 상태 메시지를 정의할 때
* **&lt;kbd&gt;** 키보드 입력 값 등의 의미를 정의할 때
* **&lt;sup&gt;** 윗첨자를 정의할 때
* **&lt;sub&gt;** 아랫첨자를 정의할 때
* **&lt;s&gt;** 텍스트에 취소선을 나타내고자 할 때
* **&lt;u&gt;** 텍스트에 밑줄을 나타내고자 할 때
* **&lt;dfn&gt;** 정의형 목록의 용어를 의미
* **&lt;ruby&gt;** 루비 요소를 삽입할 때
* **&lt;rp&gt;** 루비 요소에서 루비 괄호를 의미
* **&lt;rt&gt;** 루비 요소에서 루비 텍스트를 의미
* **&lt;bdi&gt;** 문단 내 일부 텍스트의 방향을 지정할 때
* **&lt;bdo&gt;** 텍스트의 방향(왼쪽에서 오른쪽, 오른쪽에서 왼쪽)을 지정할 때
* **&lt;span&gt;** 인라인 텍스트를 그룹화할 때
* **&lt;br&gt;** 줄바꿈하고자 할 때
* **&lt;wbr&gt;** 특정 단어 단위로 줄바꿈을 적용하고자 할 때
* **&lt;ins&gt;** 줄바꿈을 하고자 할 때
* **&lt;del&gt;** 삭제된 콘텐츠를 마크업할 때
			
## 포함 요소
* **&lt;img&gt;** 이미지를 삽입할 때
* **&lt;iframe&gt;** 인라인 프레임을 정의할 때
* **&lt;embed&gt;** 플러그인으로 실행할 외부 파일을 삽입할 때
* **&lt;object&gt;** 플러그인으로 실행할 외부 파일을 삽입할 때
* **&lt;param&gt;** &lt;object&gt; 요소의 파라미터를 지정할 때
* **&lt;video&gt;** 비디오 콘텐츠를 삽입할 때
* **&lt;audio&gt;** 오디오 콘텐츠를 삽입할 때
* **&lt;source&gt;** 비디오 및 오디오의 풀백 콘텐츠를 삽입할 때
* **&lt;track&gt;** 비디오 및 오디오의 자막이나 메타데이터를 삽입할 때
* **&lt;canvas&gt;** 동적인 비트맵 이미지를 삽입할 때
* **&lt;svg&gt;** 벡터 기반의 이미지를 삽입할 때
* **&lt;map&gt;** 이미지 맵을 정의할 때
* **&lt;area&gt;** 이미지 맵에서 링크 영역을 지정할 때
* **&lt;math&gt;** 수학 공식을 삽입할 때
	
## 테이블 요소
* **&lt;table&gt;** 테이블을 삽입할 때
* **&gt;caption&gt;** 테이블의 캡션을 정의할 때
* **&lt;colgroup&gt;** 테이블의 그룹 열을 정의할 때
* **&lt;col&gt;** 테이블의 열을 정의할 때
* **&lt;thead&gt;** 테이블의 제목 행을 정의할 때
* **&lt;tbody&gt;** 테이블의 본문 행을 정의할 때
* **&lt;tfoot&gt;** 테이블의 푸터 행을 정의할 때
* **&lt;tr&gt;** 테이블의 행을 정의할 때
* **&lt;th&gt;** 테이블의 제목 셀을 정의할 때
* **&lt;td&gt;** 테이블의 내용 셀을 정의할 때
			
## 폼 요소
* **&lt;form&gt;** 폼 서식이 포함될 영역을 마크업할 때
* **&lt;fielset&gt;** 서로 연관이 있는 폼 서식을 그룹화할 때
* **&lt;legend&gt;** 그룹화한 폼의 목적을 명시할 때

## 인터렉티브 요소
* **&lt;details&gt;** 사용자의 선택에 따라 나타내거나 숨길 수있는 영역을 정의
* **&lt;summary&gt;** 요소의 자식요소로 나타내거나 숨길 세부사항을 정의
* **&lt;dialog&gt;** 사용자의 입력이나 응답을 요구하는 팝업 등을 마크업할 때