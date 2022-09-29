## 마크다운(markdown) 작성법
---
```
박스 안의 내용은 마크다운 작성 방식이다.
```
박스 밖의 내용은 박스 안의 내용이 실제로 마크다운에서 적용된 모습이다.

## 1. 헤더(Headers)
* 글머리: 1~6까지만 지원
```
# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6
```
# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6

## 2. BlockQuote
이메일에서 사용하는 ```>``` 블럭인용문자를 이용한다.
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.

이 안에서는 다른 마크다운 요소를 포함할 수 있다.
> ### This is a H3
> - List
>	```
>	code
>	```

## 3. 목록
### ● 순서있는 목록(번호)
순서있는 목록은 숫자와 점을 사용한다.
```
1. 첫번째
2. 두번째
3. 세번째
```
1. 첫번째
2. 두번째
3. 세번째

**어떤 번호를 입력해도 순서는 내림차순으로 정의된다.**
```
1. 첫번째
3. 세번째
2. 두번째
```
1. 첫번째
3. 세번째
2. 두번째

### ● 순서없는 목록(글머리 기호: `*`, `+`, `-` 지원 / 어떤걸 써도 상관없다.)
```
* 사람
  * 학생
    * 대학생

+ Alpha
+ Bravo
+ Charlie

- 사야할 것
  - 아메리카노
  - 카페라떼
```
* 사람
  * 학생
    * 대학생

+ Alpha
+ Bravo
+ Charlie

- 사야할 것
  - 아메리카노
  - 카페라떼

혼합해서도 사용 가능하다

```
* 1단계
  - 2단계
    + 3단계
      + 4단계
```

* 1단계
  - 2단계
    + 3단계
      + 4단계

## 4. 코드
**깃헙**에서는 코드블럭코드("\```") 시작점에 사용하는 언어를 선언하여 [문법강조(Syntax highlighting)](https://docs.github.com/en/github/writing-on-github/creating-and-highlighting-code-blocks#syntax-highlighting)이 가능하다.

<pre>
<code>
```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, GDSC DAU");
  }
}
```
</code>
</pre>

```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, GDSC DAU");
  }
}
```

<pre>
<code>
```c++
#include <iostream>
int main()
{
    std::cout << "Hello, GDSC DAU" << std::endl;
    return 0;
}
```
</code>
</pre>

```c++
#include <iostream>
int main()
{
    std::cout << "Hello, GDSC DAU" << std::endl;
    return 0;
}
```


## 5. 수평선 ```<hr/>```
아래 줄은 모두 수평선을 만든다. 마크다운 문서를 미리보기로 출력할 때 *페이지 나누기* 용도로 많이 사용한다.

```
* * *
1
***
2
*****
3
- - -
4
---------------------------------------
```

* 적용예
* * *
1
***
2
*****
3
- - -
4
---------------------------------------

## 6. 링크
```
[Github](https://github.com/)
```

[Github](https://github.com/)

```
일반적인 URL 혹은 이메일주소인 경우 적절한 형식으로 링크를 형성한다.

* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>
```

* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>

## 7. 강조
```
*GDSC-DAU*
_GDSC-DAU_
**GDSC-DAU**
__GDSC-DAU__
~~GDSC-DAU~~
`GDSC-DAU`
```

- *GDSC-DAU*
- _GDSC-DAU_
- **GDSC-DAU**
- __GDSC-DAU__
- ~~GDSC-DAU~~
- `GDSC-DAU`

> ```문장 중간에 사용할 경우에는 **띄어쓰기** 를 사용하는 것이 좋다.```   
> 문장 중간에 사용할 경우에는 띄어쓰기를 사용하는 것이 좋다.


## 8. 이미지
```
![Alt text](/path/to/img.jpg)
![Alt text](/path/to/img.jpg "Optional title")
```
![석촌호수 러버덕](http://cfile6.uf.tistory.com/image/2426E646543C9B4532C7B0)
![석촌호수 러버덕](http://cfile6.uf.tistory.com/image/2426E646543C9B4532C7B0 "RubberDuck")

사이즈 조절 기능은 없기 때문에 ```<img width="" height=""></img>```를 이용한다.

예
```
<img src="/path/to/img.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
<img src="/path/to/img.jpg" width="40%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>
```

<img src="http://cfile6.uf.tistory.com/image/2426E646543C9B4532C7B0" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
<img src="http://cfile6.uf.tistory.com/image/2426E646543C9B4532C7B0" width="40%" height="30%" title="%(비율) 크기 설정" alt="RubberDuck"></img>

## 9. 줄바꿈
3칸 이상 띄어쓰기(` `)를 하면 줄이 바뀐다.

```
* 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다. 
이렇게

* 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다.___\\ 띄어쓰기
이렇게
```

* 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다. 
이렇게

* 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다.    \
이렇게

## 표

하이픈(-)는 세개이상   
:가 없을시 우측정렬   
양쪽에 :가 있을시 중앙정렬

```
|A|B|C|
|---|---|---|
|1|C++|Visual Studio|
|2|Python|Colab|

|DEF|GH|I|
|:---:|:---|---:|
|1|C++|Visual Studio|
|2|Python|Colab|
```
|A|B|C|
|---|---|---|
|1|C++|Visual Studio|
|2|Python|Colab|

|DEF|GH|I|
|:---:|:---|---:|
|1|C++|Visual Studio|
|2|Python|Colab|

## 10. HTML
- 마크다운만으로 표현이 부족하다고 느끼신다면, HTML 문법을 활용하시는 것도 좋습니다.
