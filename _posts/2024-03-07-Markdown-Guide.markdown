---
title:  "마크다운 사용법"
date:   2024-03-07 22:35:56 +0900
categories: [Blog]
tags: [markdown, 마크다운, header, 수평선, 인용구, 목록, 이스케이프, 이미지, 링크, 코드블럭, 체크리스트, 테이블]
pin: true
---

## **제목(header)**
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> `#`을 1~6개까지 사용하여 크기 조절

``` markdown
  # h1
  ## h2
  ### h3
  #### h4
  ##### h5
  ###### h6
```
<!-- 제목 출력 예시 -->
# h1
---
## h2
---
### h3
---
#### h4
---
##### h5
---
###### h6
<br><br>

## **수평선**
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> `*` 또는 `-` 또는 `_` 를 3개 이상 사용

``` markdown
  ---
  - - -
  -----
  ***
  * * *
  *****
  ___
  _ _ _
  _____
```
<!-- 수평선 출력 예시-->
  ---
  - - -
  -----
  ***
  * * *
  *****
  ___
  _ _ _
  _____
<br><br>

## **폰트 스타일(기울게/굵게/취소선)**
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> _기울여 쓰기_ : `_` 또는 `*` 한개 사용 
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> **두껍게 쓰기** : `_` 또는 `*` 두개 사용 
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> ~~취소선~~ : `~` 두개 사용 

``` markdown
  # 기울여쓰기
  hi _font style_
  hi *font style*

  # 두껍게쓰기
  hi __font style__
  hi **font style**

  # 취소선
  hi ~~font style~~

  # 혼합
  _hi_ ~~font~~ __style__
```
<!-- 수평선 출력 예시-->
  hi _font style_ <br>
  hi *font style* <br>
  - - -
  hi __font style__ <br>
  hi **font style** <br>
  - - -
  hi ~~font style~~ <br>
  - - -
  _hi_ ~~font~~ __style__

<br><br>

## **인용구**
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> `>` 로 시작하며, `>` 개수만큼 들여쓰기 가능

``` markdown
  > # 인용구 test
  >> *인용구 test*
  >>> **인용구 test**
  >>>> ~~인용구~~
  >>>>> ###### 인용구 test
```
<!-- 인용구 출력 예시 -->
> # 인용구 test
>> *인용구 test*
>>> **인용구 test**
>>>> ~~인용구~~
>>>>> ###### 인용구 test

<br><br>

## **줄바꿈**
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> `<br>` 사용
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 공백 두칸 + 엔터 

``` markdown
  안녕
  하세요
  ---
  안녕<br>
  하세요<br>
  ---
  안녕<띄어쓰기><띄어쓰기>
  하세요<띄어쓰기><띄어쓰기> 
  ---
  안녕하세요
```
<!--줄바꿈 출력 예시-->
안녕
하세요

---
안녕<br>
하세요<br>

---
안녕  
하세요   

---
안녕하세요

<br><br>

## **단락바꿈**
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 엔터 두번 연속
``` markdown
  안녕하세요<엔터><엔터>
  반갑습니다
```

<!-- 단락바꿈 출력 예시 -->
안녕하세요

반갑습니다

<br><br>

## **순서가 없는 List**
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> `*` `+` `-`를 사용

``` markdown
  * 안녕하세요
    * 순서가 없는 List
      * test 중입니다.
  + 안녕하세요
    + 순서가 없는 List
      + test 중입니다.
  - 안녕하세요
    - 순서가 없는 List
      - test 중입니다.
```
<!-- 순서가 없는 List 출력 예시 -->
* 안녕하세요
  * 순서가 없는 List
    * test 중입니다.

---
+ 안녕하세요
  + 순서가 없는 List
    + test 중입니다.

---
- 안녕하세요
  - 순서가 없는 List
    - test 중입니다.

<br><br>

## **순서가 있는 List**
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 숫자를 직접 기입해서 사용
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 각 항목의 숫자와 점 사이에 공백을 넣어야 함
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 리스트 안 리스트를 사용하려면 `Tab`과 함께 숫자 `1번`부터 나열해야 적용됨

``` markdown
  1. 사람
  2. 동물
  3. 음식
  4. 과일
    1. 오렌지
  5. 채소
    1. 토마토
```
<!-- 순서가 있는 List 출력 예시 -->
1. 사람
2. 동물
3. 음식
4. 과일
    1. 오렌지
5. 채소
    1. 토마토

<br><br>

## **백슬래쉬 이스케이프**
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 특수 문자 그대로를 사용하고자 할 때 문자 앞에 `\` 를 사용

``` markdown
  * 백슬래쉬 이스케이프
  \* 백슬래쉬 이스케이프

  - 백슬래쉬 이스케이프
  \- 백슬래쉬 이스케이프
```
<!-- 백슬래쉬 이스케이프 출력 예시 -->
* 백슬래쉬 이스케이프  

\* 백슬래쉬 이스케이프

---
- 백슬래쉬 이스케이프  

\- 백슬래쉬 이스케이프

<br><br>

## **이미지**
>#### **이미지 삽입**

``` markdown
  ![대체텍스트](/이미지파일경로)
  ![대체텍스트](이미지파일URL)
```
``` html
  <img src="이미지파일경로" alt="대체텍스트">
  <img src="이미지파일URL" alt="대체텍스트">
```
<!--이미지 삽입 출력 예시-->
![image](/assets/img/background2.jpg)

<br>

>#### **이미지 파일에 마우스를 올렸을 때 나오는 텍스트 설정**

``` markdown
  ![대체텍스트](/이미지파일경로 "커서 텍스트")
  ![대체텍스트](이미지파일URL "커서 텍스트")
```
<!--이미지 텍스트 출력 예시-->
![image](/assets/img/background2.jpg "달 사진")

<br>

>#### **이미지를 눌렀을 때 이동할 URL 설정**

``` markdown
  [![대체텍스트](이미지파일경로)](이동할 URL)
  [![대체텍스트](이미지파일URL)](이동할 URL)
```
<!--이미지 링크 출력 예시-->
[![대체텍스트](/assets/img/background2.jpg)](https://github.com/jihye046)

<br>

>#### **이미지 캡션**

<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i>`italics 폰트`로 작성하면 이미지 캡션을 달 수 있음

``` markdown
  ![image](/assets/img/background2.jpg)
  _Image Caption_
```
<!-- 이미지 캡션 출력 예시 -->
![image](/assets/img/background2.jpg)
  _Image Caption_

<br><br>

>#### **이미지 크기 조절**

<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> markdown으로 하는 경우 height 조절은 불가

``` markdown
  ![image](/assets/img/background2.jpg){: width="150px"}
```
<!-- markdown 이미지 크기 조절 출력 예시 -->
![image](/assets/img/background2.jpg){: width="150px"}

``` html
  <img src="이미지주소" alt="대체 텍스트" width="150" height="250">
```
<!-- html 이미지 크기 조절 출력 예시 -->
<img src="/assets/img/background2.jpg" alt="image" width="250" height="150">

<br><br>

## **링크**
>#### **외부 링크**

``` markdown
  [화면에 표시될 텍스트](링크 URL "마우스를 올렸을 때 보여줄 텍스트")
  [Google](http://www.google.com "구글")
  [Naver](http://www.naver.com "네이버")
```
<!-- 외부 링크 출력 예시 -->
[Google](http://www.google.com "구글") 
[Naver](http://www.naver.com "네이버")

<br>

>#### **내부 링크**

<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> `#이동할 헤드(제목)`을 쓸 때 띄어쓰기는 `-`로 연결
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> `#이동할 헤드(제목)`을 쓸 때 `()`괄호와 `/` 슬래쉬는 입력하지 않음
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> `#이동할 헤드(제목)`을 쓸 때 영어는 모두 소문자로 작성 

``` markdown
  [화면에 표시될 텍스트](#이동할 헤드(제목))
  [폰트 스타일](#폰트-스타일기울게굵게취소선)
  [순서가 없는 List](#순서가-없는-list)
```
<!--내부 링크 출력 예시 -->
[폰트 스타일](#폰트-스타일기울게굵게취소선)
[순서가 없는 List](#순서가-없는-list)

<br><br>

## **코드 블럭**
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> HTML 속성 사용 불가능(스타일 지정 불가)
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 주로 일반적인 코드 블록을 나타내는데 사용
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 백틱 3개를 앞 뒤로 붙여줌
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 백틱 옆에는 사용한 언어를 명시해줌(생략가능)

<div style="background-color: #F6F8FA; padding: 20px; border-radius: 15px; border: 1px solid #ECECEC;">
  <span class="code-block">``` java</span><br>
  <span class="code-block">&nbsp;public class Main {</span><br>
  <span class="code-block">&nbsp;&nbsp;public static void main(String[] args){</span><br>
  <span class="code-block">&nbsp;&nbsp;&nbsp;&nbsp;System.out.println("Hello, world");</span><br>
  <span class="code-block">&nbsp;&nbsp;}</span><br>
  <span class="code-block">&nbsp;}</span><br>
  <span class="code-block">```</span><br>
</div>
<!-- markdown 코드 블럭 출력 예시 -->
``` java
  public class Main {
    public static void main(String[] args) {
        System.out.println("Hello, world!");
    }
  }
```

<br><br>

## **체크 리스트**
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 완료된 리스트 표시 : `- [x]`
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 미완료된 리스트 표시 : `- [ ]`

``` markdown
  - [x] 완료된 리스트
  - [ ] 미완료된 리스트
```
<!-- 체크 리스트 출력 예시 -->
- [x] 완료된 리스트
- [ ] 미완료된 리스트

<br><br>

## **Table 테이블**
>#### **테이블 생성**

<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 헤더와 셀을 구분할 때는 `-`을 3개 사용 → `---`
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 각 열을 구분 할 때는 `|` 사용

``` markdown
  헤더1|헤더2|헤더3|헤더4
  ---|---|---|---
  칸1|칸2|칸3|칸4
  칸5|칸6|칸7|칸8
```

<!-- 테이블 출력 예시 -->

헤더1|헤더2|헤더3|헤더4
---|---|---|---
칸1|칸2|칸3|칸4
칸5|칸6|칸7|칸8

<br>

>#### **테이블 정렬**

<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 헤더의 앞 뒤 중 정렬하고싶은 위치에 `:`를 붙임
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 왼쪽 정렬 `:---`
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 가운데 정렬 `:---:`
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 오른쪽 정렬 `---:`

``` markdown
  왼쪽 정렬|가운데 정렬|오른쪽 정렬
  :---|:---:|---:
  칸1|칸2|칸3
  칸5|칸6|칸7
```
<!-- 테이블 정렬 출력 예시 -->

왼쪽 정렬|가운데 정렬|오른쪽 정렬
:---|:---:|---:
칸1|칸2|칸3
칸5|칸6|칸7





<!--
Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
-->