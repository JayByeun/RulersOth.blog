---
layout: post
author: JayB
categories: JayB
navigation: true
cover: "assets/images/cover7.jpg"
logo: "assets/images/logo.png"
tags: DevEnv
title: Regex 표현 정리
subclass: "post tag-DevEnv"
---

<br>

Regex를 사용할 때, `multiple` `global` 사용을 유의해야한다.

<br>
## 문법 정리
<br>
### Groups and ranges

| Chracter | 뜻                                     |
| -------- | -------------------------------------- |
| `\|`     | 또는                                   |
| `()`     | 그룹                                   |
| `[]`     | 문자셋, 괄호안의 어떤 문자든           |
| `[^]`    | 부정 문자셋, 괄호안의 어떤 문가 아닐때 |
| `(?:)`   | 찾지만 기억하지는 않음                 |

### Quantifiers

| Chracter    | 뜻                                  |
| ----------- | ----------------------------------- |
| `?`         | 없거나 있거나 (zero or one)         |
| `*`         | 없거나 있거나 많거나 (zero or more) |
| `+`         | 하나 또는 많이 (one or more)        |
| `{n}`       | n번 반복                            |
| `{min,}`    | 최소                                |
| `{min,max}` | 최소, 그리고 최대                   |

### Boundary-type

| Chracter | 뜻               |
| -------- | ---------------- |
| `\b`     | 단어 경계        |
| `\B`     | 단어 경계가 아님 |
| `^`      | 문장의 시작      |
| `$`      | 문장의 끝        |

### Character classes

| Chracter | 뜻                           |
| -------- | ---------------------------- |
| `\`      | 특수 문자가 아닌 문자        |
| `.`      | 어떤 글자 (줄바꿈 문자 제외) |
| `\d`     | digit 숫자                   |
| `\D`     | digit 숫자 아님              |
| `\w`     | word 문자                    |
| `\W`     | word 문자 아님               |
| `\s`     | space 공백                   |
| `\S`     | space 공백 아님              |
