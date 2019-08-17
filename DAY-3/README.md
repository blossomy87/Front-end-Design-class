# DAY-3일차 

## 1. 자간, 어간, 행간 설정


- 자간/행간 간격 

    - 자간 letter-spacing 간격 설정
    - 폰트사이즈 / 2000 (1byte 폰트조각:2000)*가로비율 (-50%)
    예) 16px/2000 * (-50%)=0.4em (em단위 사용 : font-size 상대값 대응)
    주로 제목 간격을 잡아줄 때 사용한다 

- 레이아웃 영역 (Header/Footer/Container 등) 간의 간격

    - Baseline 기준 버티컬 리듬 설정 

   
## 2. 하이퍼링크(Anchor)설정

- ₩<a href="">₩ 태그는 다른 문서와 연결(Link)하는 역할을 한다 
- HTML

'<a href="http://naver.com" target="_blank"> 네이버 사이트로 이동 </a>'<br>

- CSS

'a  {color: #34c0ff;}
 a:hover {color: #185477;} /* 마우스오버 상태 */
 a:focus {outline: 1px solid #76d8ff;} /* 키보드 접근 상태 */'<br>

## 3. 목록 리스트 설정

- '<li>' 태그 (List Item)

     - 목록의 항목 (ol, ul의 list)

- '<ol>' 태그 (Ordered List)

     - 순서가 있는 목록 

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

> 브라우저마다 'Line-Height' 영역을 정확히 못 잡을 때가 있다 
**해결방법** : `Padding`으로 남은 영역을 채워준다 (Padding-Bottom)