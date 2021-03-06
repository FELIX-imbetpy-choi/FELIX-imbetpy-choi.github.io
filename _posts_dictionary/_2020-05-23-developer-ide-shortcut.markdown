---
layout: post
title:  "[Development] IDE 란? (스크랩)-IMBETPY"
subtitle:   "The Way to become a data scientist step by step"
categories: dictionary
tags: developer ide intellij eclipse    
comments: true
---

---

![이미지](https://media.vlpt.us/images/kks1342320/post/b5a9840f-973c-44ed-8ad5-19ba5a9c7889/cover-pic.jpeg )

# Git 이란
> `Git` 은 컴퓨터 파일의 변경사항을 추적하고 여러 명의 사용자들 간에 해당 파일들의 작업을 조율하기 위한 `분산 버전 관리 시스템`이다. 소프트웨어 개발에서 소스 코드 관리에 주로 사용되지만 어떠한 집합의 파일의 변경사항을 지속적으로 추적하기 위해 사용될 수 있다.  
>  < 위키백과 > 

위의 설명이 틀린 것은 아니지만, 머리속에서 직관적으로 이해되지 않는다. 
Git을 설명할 때 보통 많이 쓰이는 비유로 다시 한번 정리 해 보자.
Git 은 버전관리 시스템이다. 이러한 버전관리는 낯설게 이 문장 속에서는 낯설게 느껴지겠지만 우리가 생활속에서 자주 마주치던 것이다.
우리가 즐기던 RPG 게임에서 게임을 진행하면서 틈틈히 시점을 저장하는 작업을 한다. 일이 잘못 되었을 때 되돌아 오기 위함이다. 또 워드 작업을 할 때에도 우리는 버전관리의 도움을 받고 있다. Ctrl+Z 를 통해서 작업한 내용을 되돌리는 때가 많기 때문이다. 타자 속도뿐 아니라, 이러한 변경점을 되돌리는 기능 또한 우리가 손글씨 보다 워드 작업이 훨씬 작업속도가 빨라 지는 이유이다. 이렇게 변경점이 관리 되는 것은 생각보다 많은 이점을 주며, 이를 전문적으로 하는 프로그램을 버전관리 시스템이라고 하며, 여러가지 프로그램이 존재한다. 하지만 여기서는 Git 만을 다룰 것이다.

https://webisfree.com/2017-12-13/git%EC%9D%B4-%EC%99%9C-%ED%95%84%EC%9A%94%ED%95%98%EB%82%98-%EB%B0%98%EB%93%9C%EC%8B%9C-%EC%8D%A8%EC%95%BC%ED%95%98%EB%8A%94%EA%B0%80

https://git-scm.com/book/ko/v2 

https://linked2ev.github.io/devlog/2018/08/27/Git-1.-What-is-Git/

https://books.google.co.kr/books?id=nffJDwAAQBAJ&pg=PA212&lpg=PA212&dq=git+cli+%EC%99%9C?&source=bl&ots=OdbTBaAlf9&sig=ACfU3U0Dyz4OLlCYcE3ug91iTQg5SP5jig&hl=ko&sa=X&ved=2ahUKEwjJzsqaorLpAhUVPnAKHe_aBZ0Q6AEwCHoECAoQAQ#v=onepage&q=git%20cli%20%EC%99%9C%3F&f=false

<br/>
<br/>

---


# Git 왜 사용해야 하나?
+ ## 장점👍
    1. 문법이 간결하고, 특별한 도구 없이 작성이 가능하다.
    2. 텍스트 파일 형태로 관리가 쉽다. (버전관리 또한 가능)
    3. 여러 플랫폼과 프로그램에서 사용이 가능하다. 
        - 워드프레스(WordPress) 
        - 텀블러(Tumblr) 
        - 레딧(Reddit) 
        - 깃허브(GitHub) 
        - 스택오버플로우(Stack Overflow) 
        - 주피터노트북(Jupyter notebook) 
        - velog 

+ ## 한계👎
    1. 문법이 간결기 때문에, 범위에서 벗어나는 기능은 HTML 을 사용해야 한다.
    2. 표준이 없다. 여러 확장문법이 등장하면서 플랫폼에 따라 작동하지 않는 문법이 있다.
    3. 멀티미디어 삽입이 불편하다. 


<br/>
<br/>

---


# 그럼 왜 CLI 를 사용하나?

`h1` 부터 `h6` 까지 표현할 수 있으며, `#` 의 개수에 따라 제목의 크기(계층)을 지정합니다.  

✏️ 마크다운 CODE
```
# h1
## h2
### h3
#### h4
##### h5
###### h6
```

💻 결과값 Console
# h1
## h2
### h3
#### h4
##### h5
###### h6


<br/>
<br/>

---


# 2. 목록(List)

## 2-1. 글머리 목록(Bulleted list)
`순서가 없는 목록` 을 나열할 때 사용하며, `-`, `*`, `+` 로 작성합니다.  
Tab 이나 스페이스바를 이용하여 들여쓰기가 가능합니다.


✏️ 마크다운 CODE
```
+ 1계층
    - 2계층
      * 3계층
        + 4계층
```

💻 결과값 Console
+ 1계층
    - 2계층
      * 3계층
        + 4계층

## 2-2. 번호 목록(Numbered list)
`숫자 목록` 을 나열할 때 사용하며, `숫자`와 `.` 로 작성합니다.  

✏️ 마크다운 CODE
```
1. 첫번째
2. 두번째
3. 세번째
```

💻 결과값 Console
1. 첫번째  
2. 두번째   
3. 세번째   


<br/>
<br/>

---


# 3. 인용문(Quote)

`인용문` 이나 `요약` , `강조` 등을 표현할 때 사용하며,  `>` 로 작성합니다.

✏️ 마크다운 CODE
```
> Who is wise? He that learns from every One. Who is powerful? He that governs his Passions. Who is rich? He that is content. Who is that? Nobody.  
-Benjamin Franklin


> 중첩 1계층
>> 중첩 2계층
>>> 중첩 3계층
```

💻 결과값 Console
> Who is wise? He that learns from every One. Who is powerful? He that governs his Passions. Who is rich? He that is content. Who is that? Nobody.   
-Benjamin Franklin


> 중첩 1계층
>> 중첩 2계층
>>> 중첩 3계층

<br/>
<br/>

---


# 4. 폰트스타일 & 줄바꿈

`줄바꿈` 은 문장 마지막에 (spacebar)(spacebar) 2번, (Enter) 를 적용해야 줄이 변경됩니다.  
여러줄을 추가 하려면 HTML 태그 `<br/>` 을 사용하면 됩니다.

✏️ 마크다운 CODE
```
__볼드__   
**볼드**   
_기울임체_  
*기울임체*  
~~취소선~~  
<u>밑줄</u>    
__볼드구역 *이탤릭구역* 볼드구역__  
`인라인코드`

개행
미완료

개행(spacebar)(spacebar)   
완료

개행<br/>
완료
```

💻 결과값 Console  

__볼드__   
**볼드**   
_기울임체_  
*기울임체*  
~~취소선~~  
<u>밑줄</u>    
__볼드구역 *이탤릭구역* 볼드구역__  
`인라인코드`

개행
미완료  

개행(spacebar)(spacebar)   
완료

개행<br/>
완료


<br/>
<br/>

---


# 5. 코드블럭(Code Blocks)
코드를 삽입할 때 사용하며, `백틱(｀)` 을 3개 사용하여 작성합니다.  
백틱(`) 뒤에 개발언어를 나타내주면 언어에 맞는 하이라이트가 드러납니다.  

✏️ 마크다운 CODE
```
```　
백택3개 이상(```)을 위,아래에 작성하면 코드블럭이 만들어진다.
```　
```

```
```java
public static void main(String[] args) {

		int sum1 = 1;
		int sum2 = 2;
		
		int res = sum1 + sum2;
		
		System.out.println(res);
	}
```　
```

💻 결과값 Console  

```
백택3개 이상(```)을 위,아래에 작성하면 코드블럭이 만들어진다.
```

```java
public static void main(String[] args) {

		int sum1 = 1;
		int sum2 = 2;
		
		int res = sum1 + sum2;
		
		System.out.println(res);
	}
```


<br/>
<br/>

---


# 6. 링크(Link)
클릭 시 다른 페이지로 이동하며, 3가지 다른 유형이 존재합니다.

✏️ 마크다운 CODE
```
(유형1)  
`링크제목 지정` : 
[네이버](https://felix-imbetpy-choi.github.io/ "설명어")  

(유형2) 
`링크URL 노출` : <https://felix-imbetpy-choi.github.io/> 

(유형3) 
`동일파일 링크(목차)` : [목차](##개요) 
```

> __`<유형3> 문단 링크 방법`__  
> 0. 링크는 h1(#) 이 적용된 제목만 가능하다.  
> 1. 링크 할 제목(header)을 복사,붙여넣기   
> 2. `특수문자`제거    
> 3. 스페이스를 갯수만큼 `-`로 변경    
> 4. 대문자->`소문자`로 변경     
> ex) "#목차?  !장점" -> "#목차--장점"  



💻 결과값 Console  


(유형1)  
`링크제목 지정` : 
[네이버](https://felix-imbetpy-choi.github.io "설명어")  

(유형2)   
`링크URL 노출` : <https://felix-imbetpy-choi.github.io> 

(유형3)   
`동일파일 링크(목차)` : [목차](##개요)  


<br/>
<br/>

---


# 7. 이미지(Image)
마크다운을 사용하여 `이미지를 삽입`할 땐 사이즈 조절이 불가능합니다.     
때문에 `사이즈 조절`이 필요할 땐 `HTML` 을 사용하면 됩니다.  
또한 이미지에 링크 적용이 가능합니다.     

✏️ 마크다운 CODE
```
(유형1) 이미지 삽입
![이미지](https://topclass.chosun.com/news_img/1807/1807_008.jpg "냐옹이")
  
(유형2) 이미지 사이즈 조절
<img src="https://topclass.chosun.com/news_img/1807/1807_008.jpg" width="300" height="200"> 

(유형3) 이미지 링크
[![이미지](https://topclass.chosun.com/news_img/1807/1807_008.jpg)](https://felix-imbetpy-choi.github.io/)  
```

💻 결과값 Console  

(유형1) 이미지 삽입  
![이미지](https://topclass.chosun.com/news_img/1807/1807_008.jpg "냐옹이")
  
(유형2) 이미지 사이즈 조절  
<img src="https://topclass.chosun.com/news_img/1807/1807_008.jpg" width="300" height="500"> 

(유형3) 이미지 링크  
[![이미지](https://topclass.chosun.com/news_img/1807/1807_008.jpg)](https://felix-imbetpy-choi.github.io/)  


<br/>
<br/>

---


# 8. 테이블(Table)
`표형식` 을 삽입할 때 사용하며, `|` , `:` , `-` 를 통해서 작성합니다.   
테이블 헤더를 작성하고, 아래줄에는 구분선(`-`) 과 정렬(`:`) 을 표시한다.    
`:` 를 왼쪽, 양쪽, 오른쪽에 표기하여 왼쪽, 가운데, 오른쪽 정렬을 구현한다.

✏️ 마크다운 CODE
```
| 트레이닝 날짜 | 트레이닝 종류 | 트레이닝 강도 |
|:----------|:----------:|----------:|
| 2020.05.05 | **푸쉬업**, 벤치프레스 | 20*5set, 15*6set |
| 2020.05.07 | _풀업_, 바벨로우, 랫풀다운 | 9*5set, 20*5set, 15*5set,|
| 2020.05.09 | 달리기, 복근운동 | ~~40min~~, 20*5set, |
```

💻 결과값 Console  

| 트레이닝 날짜 | 트레이닝 종류 | 트레이닝 강도 |
|:----------|:----------:|----------:|
| 2020.05.05 | **푸쉬업**, 벤치프레스 | 20*5set, 15*6set |
| 2020.05.07 | _풀업_, 바벨로우, 랫풀다운 | 9*5set, 20*5set, 15*5set,|
| 2020.05.09 | 달리기, 복근운동 | ~~40min~~, 20*5set, |


<br/>
<br/>

---


# 9. 이모지(Emoji)

글과 양식만을 이용해 작성하면 너무 딱딱해 보이기 쉽습니다.  
`윈도우`나 `맥` 에서도 기본적으로 사용할 수 있는 `이모지`를 알아보고,  
`이모지` 를 제공하는 사이트를 소개합니다.  

- 트위터 및 텍스트 이모지 사이트  
https://kr.piliapp.com/twitter-symbols

+ 단축키
    - window10 : `윈도우키` + `마침표(.)`
    - mac : `Command` + `Control` + `스페이스바`

<br/>
<br/>

---


# 마침🙌🏿

jeklly 을 통해 작성하는 첫 글 입니다.   
첫 글 주제로 블로그를 작성하면서 계속 마주칠 마크다운에 대해서 알아보고, 정리해 보았습니다.  
아주 기초적인 내용을 정리했고, 추가적으로 필요한 문법은 수정하려고 합니다.  
위의 본문에 없지만 필수적이라고 생각되는 문법이 있다면 댓글에 남겨주세요~!~! 🎈



<br/>
<br/>

---


# 참고📚
- <https://gist.github.com/ihoneymon/652be052a0727ad59601>

<br/>
<br/>

---

