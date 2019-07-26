# DAY-2일차 

## 1. 제목 설정 (H1~H6)

> max-width : 1366px 기준 , 본문 폰트 16px 로 설정

- 기본 제목 설정

    - 브라우저 기본 사이즈는 '16px' 기준으로 (H1 - H4)의 스케일은 상향되고, (H5 -H6)의 스케일은 하향된다


- 제목 크기 (기본 16px 기준)

    <H1> `H1` font-size: 32px , 2em <br>
    <H2> `H2` font-size: 24px , 1.5em <br>
    <H3> 'H3` font-size: 19px , 1.33em <br>
    <H4> `H4` font-size: 16px , 1.17em <br>
    <H5> `H5` font-size: 13px , 0.83em <br>
    <H6> `H6` font-size: 11px , 0.67em <br>
<br>

## 2. 본문 설정 (Paragraph)

- 브라우저 기본 폰트 사이즈 
    - 16px / 1.2 기본 설정

> 대부분의 브라우저 폰트 사이즈의 기본 값은 12pt, 16px, 1em, 100% 이다 <br>

- 국문, 영문 폰트 사이즈 
    - 국문 폰트 13~14px 사용
    - 영문 폰트 16px 사용 

- 웹 폰트 설정 사용 단위 'px, em, rem, %, vw, vh'

      '절대 단위 (absolute)' : px, pt
      '상대 단위 (relative)' : em, rem, %, vw, vh

     - **em** : 엘리먼트의 폰트 크기를 결정한다 <br><br>
     >**font-size: 1.5em;** 은 글자 크기를 `상위 요소 크기의 1.5`배로 하겠다는 것을 뜻한다 

       `ex) 16(px) x 1.5(em) = 24px`

     - **rem(Root em)** : 루트 엘리먼트(html)의 폰트 크기를 결정한다 <br><br>
     >**font-size: 1rem;** 은 html (or body)에서 설정한 폰트 크기를 기준으로 계산된다 

       `ex) html { font-size : 16px; }
            div { font-size : 20px; width : 10rem; }`/*160*/

- 단위 공식 
    - PX to REM = size in pixels / root size pixel<br>
    ex) 16px / 10px(body) = 1.6rem

   - PX to EM = size in pixels / parent size in pixel<br>
    ex) 12px / 16px = 0.75em

   - PX to % = size in pixels / parent size in pixels<br>
    ex) 12px / 16px * 100 = 75%

   - PX to PT = size in pixels * (points per inch / pixels per inch)<br>
    ex) 16px * (72pt / 96px) = 12pt

   - EM to PX = size in EMs * parent size in pixels<br>
    ex) 0.75em * 16px = 12px

   - EM to % = size in EMs * 100<br>
    ex) 0.75em * 100 = 75%

<br>
            
### 참고

- [Grid Lover](https://www.gridlover.net/try)
- [px/em 단위계산](http://pxtoem.com/)
- [Reset CSS](https://meyerweb.com/eric/tools/css/reset/)
<br>

## 3. 자간, 행간 설정 

- Text 기준 : `Base-Line (Line-Height)`
- 레이아웃, 레이어, 컨테이너 기준 : `Base-Line (Height Gap)`

> 브라우저마다 'Line-Height' 영역을 정확히 못 잡을 떄가 있다 
**해결방법** : `Padding`으로 남은 영역을 채워준다 (Padding-Bottom)