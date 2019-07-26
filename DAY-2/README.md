# DAY-2일차 

## 1. 제목 설정 (H1~H6)

> 대부분의 브라우저 폰트 사이즈의 기본 값은 12pt, 16px, 1em, 100% 이다 <br>
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

## 2. 웹 폰트 설정 단위 
- 웹 폰트 설정 사용 단위 'px, em, rem, %, vw, vh'

      '절대 단위 (absolute)' : px, pt
      '상대 단위 (relative)' : em, rem, %, vw, vh

     - **em** : 엘리먼트의 폰트 크기를 결정한다 <br><br>
     >**font-size: 1.5em;** 은 글자 크기를 `상위 요소 크기의 1.5`배로 하겠다는 것을 뜻한다 

       `ex) 16(px) x 1.5(em) = 24px`

     - **rem(Root em)** : 루트 엘리먼트(html)의 폰트 크기를 결정한다 <br><br>
     >**font-size: 1rem;** 은 html (or body)에서 설정한 폰트 크기를 기준으로 계산된다 

       `ex) html { font-size : 16px; }<br>
            div { font-size : 20px; width : 10rem; }<br>
            **16 x 10 = 160px** 본문 기준으로 계산한다` <br>

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
            

![](http://pxtoem.com/)
<br>

