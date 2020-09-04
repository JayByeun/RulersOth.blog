---
layout: post
author: JayB
categories: JayB
navigation: true
cover: 'assets/images/cover7.jpg'
logo: 'assets/images/logo.png'
tags: DevEnv
title: Writing with markdown
subclass: 'post tag-DevEnv'
---

> 마크다운은 <strong>html보다</strong> 쉬운 온라인 문서 작성방법이다. 마크다운으로 작성된 문서는 html로 변환이 쉬워 블로그나 간편한 웹 문서를 만들기에 적합하다. 하지만 마크다운 문서는 작성이 쉬운 반면, 웹 상에서 올바른 형식으로 인식하지 못하는 경우가 많기 때문에 자동으로 html 문서 형식으로 변환해 주는 과정이 필요하다. 이 대표적인 툴이 깃헙 블로그를 만들때 쓰이는 <strong>jekyll 이다.</strong><br> - 내가 공부한 건 그렇다.

***
#### 1. Heading 편집
소제목과 같이 하이라이트가 필요한 경우 '#, -, =' 사용할 수 있다.
```
 # heading
 ## heading
 heading
 --
 heading
 ==
 ...
 ```
# Heading
## Heading
### Heading
#### Heading
##### Heading
###### Heading

heading
-
heading
=====

#####   1.1 강조
```
강조효과는 *asterisks* or _underscores_ 사용한다.
강한 강조 효과는 두개씩 양쪽에 사용 **asterisks** or __underscores__.
취소선은 ~~Scratch this.~~

```
강조효과는 *asterisks* or _underscores_ 사용한다. <br>
강한 강조 효과는 두개씩 양쪽에 사용 **asterisks** or __underscores__. <br>
취소선은 ~~Scratch this.~~ <br>

***
#### 2. 줄바꿈
줄바꿈 서식은 <br>을 사용해서 적용할 수 있다.
```
언젠가 나도 이 페이지를 안보고 바로 마크다운 문서를<br>
작성할 수 있을까요?
```
언젠가 나도 이 페이지를 안보고 바로 마크다운 문서를<br>
작성할 수 있을까요?

#### 3. 인용문구 묶기
인용 문구는 '>'를 이용해서 묶어서 표현할 수 있다.
```
> I Disapprove of What You Say, <br>
But I Will Defend to the Death Your Right to Say It <br> -Voltaire
```
> I Disapprove of What You Say, <br>
But I Will Defend to the Death Your Right to Say It <br> -Voltaire

#### 4. 실선 넣기
실선은 '*, -, _'를 사용해서 표현할 수 있다.
```
기호들을 3개 이상씩 써주면 된다.
***
---
___
```
***
---
___

#### 5. 코드 블럭 넣기
코드 블럭 효과는 '`'를 사용해서 표현할 수 있다.
```
계속 쓰고 있었는데 이렇게 ```를 세개씩 사용하면 전체 문단을 블럭할 수 있다.
`세개 뒤에 프로그래밍 언어를 쓰면, 아래와 같이 코드를 블럭해서 표현할 수 있다.
```
```java
@Override
    public void execute() {
        try {
            game.place(from, to);
            ReadWrite.writeLine(InOutputStrings.POSITIVE);
        } catch (GameLogicException e) {
            ReadWrite.writeError(e.getMessage());
        }
    }
```
`한 문장만 블럭하기`

***

#### 6. 링크 넣기
링크는 세가지 종류가 있다.
```
1) 인라인 링크
[RulersOth](http://RulersOth.github.io)
2) url 삽입
<http://RulersOth.github.io>
3) reference 삽입
Some links need references.
[Some links]:(http://RulersOth.github.io)
```
● 인라인 링크<br>
[RulersOth](http://RulersOth.github.io)<br>
● url 삽입<br>
<http://RulersOth.github.io><br>
● reference 삽입<br>
[Some links need references.][1] <br>
[1]:(http://RulersOth.github.io/) <br>

***

#### 7. 표 만들기
표는  콜론(:)과 dash(-)를 이용해 구성한다. 콜론은 칼럼을 연결하고 dash는 헤드 셀을 구분한다.
Pipes(|)는 칼럼을 구분한다.  마지막 파이프는 생략 가능하다.
```
Number | *name* | status |
------:|-----:|-------:|
1 | mark | down |
```

Number | *name* | status |
------:|-----:|-------:|
1 | mark | down |

***

#### 8. 글자 색상 변경
글자 색상은 html을 작성해서 변경 할 수 있다.
```
<span style="color:blue">the color is blue</span>
<span style="color:#D07111">#D07111</span>
<span style="color:rgb(123, 200, 5)">different setting of rgb</span>
```
<span style="color:blue">the color is blue</span> <br>
<span style="color:#D07111">#D07111</span> <br>
<span style="color:rgb(123, 200, 5)">different setting of rgb</span> <br>





***

##### ◼︎ Reference
[Github Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
