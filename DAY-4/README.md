# DAY-4일차

## 1. 그리드 시스템

![반응형 그리드 시스템](../image/readme_responsive_ex.png)

## 그리드 시스템 설정 공식

- 컬럼 폭 구하는 공식
    -( 최대폭(Grid) 너비 - ( 거터 폭 * ( 컬럼 수 - 1 )) / 컬럼 수 = 컬럼 폭

- 최대폭(grid) 너비 구하는 공식 */
    -( 컬럼 폭 * 컬럼 수 ) + ( 거터 폭 * (컬럼 수 - 1)) = 최대폭(Grid) 너비

- 마진(여백) 구하는 공식
    -( 중단점(breakpoint) 너비 - 최대폭(Grid) 너비 ) / 2

- 컬럼 값 픽셀 단위 퍼센트로 구하는 공식
    -( 컬럼 폭 / 최대폭(Grid) ) * 100%

## 2. 레이아웃 중단점 설정 방법

- Desktop, Tablet, Mobile 기준 중단점 (BreakPoint)을 설정
- Columns : 컬럼 수
- Gutter : 컬럼 사이 공간
- Max Width : 중단점 (변화시점)
- Margin : 레이아웃 여백

## 3. 디바이스별 그리드 시스템 설계

- Desktop
    -컬럼 (12) / 거터 (20px) / 최대 폭 (1360px) / 마진 (90px)
- Tablet
    -컬럼 (6) / 거터 (20px) / 최대 폭 (768px) / 마진(76px)
- Mobile
    -컬럼 (4) / 거터 (20px) / 최대 폭 (480px) / 마진 (24px)

```css
a  { color: #34c0ff;}
a:hover {color: #185477;} /* 마우스오버 상태 */
 a:focus {outline: 1px solid #76d8ff;} /* 키보드 접근 상태 */
 ```
 <br>

## 3. 목록 리스트 설정

- `<li>` 태그 (List Item)

     - 목록의 항목 (ol, ul의 list)

- `<ol>` 태그 (Ordered List)

     - 순서가 있는 목록 

- HTML
```html
<ol>
    <li>리스트1</li>
    <li>리스트2</li>
</ol>
````
<br>


- `<ul>` 태그 (UnOrdered List)

     - 순서가 없는 목록 

- HTML
```html
<ul>
    <li>리스트</li>
    <li>리스트</li>
</ul>
````

<br>

- `<dl>` 태그 (Definition List)
	- 정의 목록(용어 목록)

- `<dt>` 태그 (definition term)
  - 정의 용어(용어 제목)

- `<dd>` 태그 (definition description)
  - 정의 설명(용어 설명)

- HTML
```html
<dl>
  <dt>정의 1</dt>
  <dd>정의 1</dd>
  <dt>정의 2</dt>
  <dd>정의 2 </dd>
</dl>
```

### 레이아웃 구성

- Header 영역
  - 웹페이지를 나타내는 로고 또는 소개글
  - `<header>` 영역 태그

- Navigation 영역
  - 웹페이지에서 다른 페이지로 이동하는 메뉴
  - `<nav>` 영역 태그

- Conteiner 영역
  - 웹 페이지의 내용(Content)
  - `<section>`, `<article>`, `<aside>` 영역 태그

- Footer 영역
  - 웹 페이지와 관련된 정보
  - `<footer>` 영역 태그


### 리셋(Reset)CSS 작성 

- 폰트 설정 
  - `10px`로 계산하는 것이 더 편리하다 
  - 이후 자간,행간 설정 시 Padding값을 별도로 지정하며 조절한다 

- `reset.css`는 최소한으로 설정 
  - 프로젝트별 reset.css를 추가 구성 해줄 수 있다 


### Float / Display 를 활용한 단락 나누기

- `display-inline-block``
  - width / height 값 설정이 필요하다 
  - 반응형일 경우 `max-width를 사용

> Display 빈 공간 없애기 

``` 
부모 (최상위 단위)에 폰트 빈 공간을 0으로 변경 후 본문 폰트를 별도로 설정한다 
```

<br>

- `float-left;``
  - 단을 아래로 내리려면 최상위 부모에게 "clear-both;" 설정을 해준다