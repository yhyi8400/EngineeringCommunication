Markdown Language
==============

2.1 Header
------------

# This is a H1

## This is a H2

### This is a H3

#### This is a H4

##### This is a H5

###### This is a H6


2.2 BolckQuote
----------------

> This is a first blockqute.

>	> This is a second blockqute.

>	>	> This is a third blockqute.


2.3 List
--------

순서가 있는 목록

숫자와 점을 사용

1. 첫번째 목록
	- 순서가 없는 목록
	- 순서가 없는 목록
1. 두번째 목록
1. 세번째 목록



순서가 없는 목록(글머리 기호: *, +, -)

* Blue
  * Green
    * Red

+ Blue
  + Green
    + Red

- Blue
  - Green
    - Red


* 1st Stage
  - 2nd Stage
    + 3rd Stage
      + 4th Stage


2.4 Code
---------

2.4.1 들여쓰기
---------------

2022/06/21(화) 누리호 발사 성공

	세계에서 7번째 우주 강국

누리호 성공 축하!!!! 	


2022/06/21(화) 누리호 발사 성공
	세계에서 7번째 우주 강국
누리호 성공 축하!!!! 


2.4.2 Code Block
------------------

* { <pre><code>  {code}  </code></pre> } 이용방법

<pre>
<code>
class Car {
    private String modelName;
    private int modelYear;
    private String color;
    private int maxSpeed;
    private int currentSpeed;

    Car(String modelName, int modelYear, String color, int maxSpeed) {
        this.modelName = modelName;
        this.modelYear = modelYear;
        this.color = color;
        this.maxSpeed = maxSpeed;
        this.currentSpeed = 0;
    }
}
</code>
</pre>	

* "  '''  {code}  '''  " 이용방법

```
import React from 'react';

function MyComponent(props) {
  if (props.isBar) {
    return <div>Bar</div>;
  }

  return <div>Foo</div>;
}

export default MyComponent;
```

* 코드블럭 시작점("  ''' ")에  사용하는 언어를 선언하여 문법 강조 가능

```js 
import React from 'react';

function MyComponent(props) {
  if (props.isBar) {
    return <div>Bar</div>;
  }

  return <div>Foo</div>;
}

export default MyComponent;
```


2.5 Draw Line
---------------

* * *
***
*****
- - - 
---------------

2.6 Link
---------------

* 참조 링크

// examle

Link: [google][googlelink]

[googlelink]: https://google.co.uk "Let's Go Google"


* 외부 링크

// examle

[Google](https://google.co.uk "Let's Go Google")



* 자동 링크

// examle

Google Homepage: https://google.co.uk 

Naver Homepage: <https://naver.com>


2.7 Emphasis
---------------

// examle

이텔릭체 *별표(asterisks)* 혹은 _언더바(underscore)_ 사용

두껍게는 **별표(asterisks)** 혹은 __언더바(underscore)__ 사용

**_이텔릭체_와 두껍게**를 같이 사용할 수 있음

취소선은 ~~물결표시(tilde)~~ 를 사용

<strike>취소선</strike>은 <s>stike</s> 또는 <del>del</del>를 사용하세요. 


2.8 Image
-----------

![Street](TestImage.jpg "Oxford")

Inline-style: 
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Reference-style: 
![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"

'크기 조절'

<img src="TestImage.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
<img src="TestImage.jpg" width="40%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>


2.9 Footnotes
--------------

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].  

You can also use words, to fit your writing style more closely[^note].

[^1]: My reference.
[^2]: Every new line should be prefixed with 2 spaces.  
  This allows you to have a footnote with multiple lines.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.  
    This footnote also has been made with a different syntax using 4 spaces for new lines.

2.10 Table
--------------

| 값 | 의미 | 기본값 |
|---|:---:|---:|
| `static` | 유형(기준) 없음 / 배치 불가능 | `static` |
| `relative` | 요소 자신을 기준으로 배치 |  |
| `absolute` | 위치 상 부모(조상)요소를 기준으로 배치 |  |
| `fixed` | 브라우저 창을 기준으로 배치 |  |


Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3


2.11 줄바꿈
--------------

*일반 텍스트 문장:  문장 끝에 공백 2번(스페이스 2번)하면 줄 바꿈이 됨.  
예를 들어, 지금  
공백 2번 만들어서 지금과 공백 사이에서 줄바꿈이 된다.

*테이블 내에서나 일반적인 경우:  "<br> 사용"  
안녕하세요. <br>반갑습니다. 줄이 바뀌었어요.