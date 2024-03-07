---
layout: post
title:  "블로그 사용법"
date:   2024-03-07 23:07:58 +0900
categories: [Blog]
tags: [blog, 마크다운, markdown, liquid, 코드블럭]
pin: true
---
## **코드 블럭**

>#### **liquid 사용**

<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> HTML 속성 사용 가능(스타일 지정 가능)
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 스타일을 지정하고자 할 때는 `raw` 와 `endraw` 로 감싸주어야 함
<br>
<i class="fa-solid fa-pencil fa-bounce" style="color: #b3b5bc;"></i> 주로 문서나 블로그 코드에 하이라이팅(색상 강조)을 적용할 때 사용

[스타일 지정하는 경우]
<div style="background-color: #F6F8FA; padding: 20px; border-radius: 15px; border: 1px solid #ECECEC;">
  <span class="code-block">&#123;% raw %&#125;</span><br>
  <span class="code-block">&#123;% highlight ruby %&#125;</span><br>
  <span class="code-block">코드</span><br>
  <span class="code-block">&#123;% endhighlight %&#125;</span><br>
  <span class="code-block">&#123;% endraw %&#125;</span>
</div>
<br>
[스타일 지정 안 하는 경우]
<div style="background-color: #F6F8FA; padding: 20px; border-radius: 15px; border: 1px solid #ECECEC;">
  <span class="code-block">&#123;% highlight ruby %&#125;</span><br>
  <span class="code-block">코드</span><br>
  <span class="code-block">&#123;% endhighlight %&#125;</span><br>
</div>
<br><br>

>#### **markdown 사용**

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