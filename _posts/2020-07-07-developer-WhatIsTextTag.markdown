---
layout: post
title:  "[HTML5] 3 HTML Text Tag? 소개-IMBETPY"
subtitle:   "About Text Tag"
categories: developer
tags: what is Text Tag Tag in internet
comments: true
---
## 개요
> `Text Tag` 의 개념과 종류를 정리했습니다.

---


![](https://images.velog.io/images/doomchit_3/post/af55ccb6-c11f-453f-91d4-43bde041c4f4/image.png)

# 🎫 제목 (Headings) 태그
- `Heading태그` 는 제목을 나타낼 때 사용하며 **h1에서 h6까지**의 태그가 있다. 
- h1 태그는 가장 크기가 크며, 제목을 나타낸다. 
- 검색엔진은 제목 태그를 중요한 의미로 받아들일 가능성이 크다. 

```
<!DOCTYPE html>
<html>
  <body>
    <h1>heading 1</h1>
    <h2>heading 2</h2>
    <h3>heading 3</h3>
    <h4>heading 4</h4>
    <h5>heading 5</h5>
    <h6>heading 6</h6>
  </body>
</html>
```

<br/>
<br/>

# 🀄 글자 형태 (Text Formatting) 태그
### ① b
- **bold체를 지정** 한다. 
- 제목 태그와 같이 의미론적(Semantic) 중요성의 의미는 없다.
```
    <b>bold.</b>

```

### ② strong
- b tag와 동일하게 **bold체를 지정** 한다. 
- 의미론적(Semantic) 중요성의 의미를 갖는다.
- 표현되는 외양은 b tag와 동일하지만 웹표준을 준수하고자 한다면 strong를 사용하는 것이 바람직하다.
```
    <strong>strong.</strong>
    
```

### ③ i
- **Italic체를 지정** 한다. 
- 의미론적(Semantic) 중요성의 의미는 없다.
```
    <i>italic.</i>

```


### ④ em
- **emphasized(강조, 중요한) text를 지정** 한다. 
- i tag와 동일하게 Italic체로 표현된다. 
- 의미론적(Semantic) 중요성의 의미를 갖는다.
```
    <em>emphasized.</em>

```

### ⑤ small
- **small text를 지정** 한다.
```
    <h2>HTML <small>Small</small> Formatting</h2>

```


### ⑥ mark
- **highlighted text를 지정**한다.

```
    <h2>HTML <mark>Marked</mark> Formatting</h2>
```

### ⑦ del
- **deleted (removed) text를 지정**한다.
```
    <p>My name is <del>junyeong</del> hello.</p>

```


### ⑧ ins
- **inserted (added) text를 지정** 한다.
```
    <p>My my <ins>name</ins> is junyeong.</p>

```


### ⑨ sub / sup
- sub 태그는 subscripted(아래에 쓰인) text를 
- sup 태그는 superscripted(위에 쓰인) text를 지정한다.
```
  <p>hello<sub>my</sub> world.</p>
  <p>hello<sup>my</sup> world.</p>
```

<br/>
<br/>

# 🏮 본문 태그
### ① p
- **단락 (Paragraphs)을 지정**한다.
```
    <p>1단락.</p>
    <p>2단락.</p>
```

### ② br
- **강제개행을 지정** 한다. 
- br tag는 빈 요소(empty element)로 종료태그가 없다.
```
    <p>hello<br>a<br>boy</p>

```
- HTML에서는 1개 이상의 연속된 공백(space)을 삽입하여도 1개의 공백으로 표시된다. 
- 1개 이상의 연속된 줄바꿈(enter)도 1개의 공백으로 표시된다. 
- 연속적 공백을 삽입하는 방법은 `&nbsp;` 를 사용한다.

```
    <p>This is&nbsp; a para&nbsp; &nbsp; graph</p>

```


### ③ pre
- 형식화된(preformatted) text를 지정한다. (코드를 삽입할 때 많이 사용)
- pre 태그 내의 content는 작성된 그대로 브라우저에 표시된다.
```
<pre>
var myArray = [];
console.log(myArray.length); // 0

myArray[1000] = true;  // [ , , ... , , true ]

console.log(myArray.length); // 1001
console.log(myArray[0]);     // undefined
    </pre>
```

### ④ hr
- 수평줄을 삽입한다.
```
    <hr>

```

### ⑤ q
- 짧은 인용문(quotation)을 지정한다. 
- 브라우저는 인용부호(큰따옴표/quotation marks)로 q 요소를 감싼다.
```
    <p> Well done is better than well said. (Benjamin Franklin) </q></p>

```

### ⑥ blockquote
- 긴 인용문 블록을 지정한다.
- 브라우저는 blockquote 요소를 들여쓰기한다. 
- css를 이용하여 다양한 style을 적용할 수 있다.
```
<blockquote>
      <p>It is the working man who is the happy man. It is the idle man who is the miserable man. (Benjamin Franklin) </p>
    </blockquote>
```

<br/>
<br/>

# 참고📚
[mozilla](https://developer.mozilla.org/ko/docs/Web/HTML)
[poiemaweb](https://poiemaweb.com)