# Markdown syntax guide
**마크다운(Markdown)**은 경량 마크업 언어  
간단한 텍스트 기반 문법으로 문서 서식을 표현 가능  
파일 확장자 - README.md  

## 1. 제목(Header)
######제목은 6개까지 가능하고 #뒤는 띄어쓰기 해야합니다.
```
# 제목1
## 제목2
### 제목3
#### 제목4
##### 제목5
###### 제목6
```

# 제목1
## 제목2
### 제목3
#### 제목4
##### 제목5
###### 제목6


## 2. 강조
```
**굵게**    또는    __굵게__

*기울임*    또는    _기울임_

~~취소선~~

__*이텔릭체*와 두껍게__ 를 혼용할 수도 있습니다.
```

**굵게**    또는    __굵게__

*기울임*    또는    _기울임_

~~취소선~~

__*이텔릭체*와 두껍게__ 를 혼용할 수도 있습니다.


## 3. 목록

```markdown
1. 순서가 있는 항목
1. 순서가 있는 항목
<tab> 1. 순서가 없는 항목
<tab> 1. 순서가 없는 항목
1. 순서가 있는 항목
1. 순서가 있는 항목

- 순서가 없는 항목
- 순서가 없는 항목
<tab> - 순서가 없는 항목
<tab> - 순서가 없는 항목
```

1. 순서가 있는 항목
1. 순서가 있는 항목
    1. 순서가 없는 항목
    1. 순서가 없는 항목
1. 순서가 있는 항목
1. 순서가 있는 항목

- 순서가 없는 항목
- 순서가 없는 항목
    - 순서가 없는 항목
    - 순서가 없는 항목

## 4. 링크와 이미지
### Images
```
![대체 텍스트(Alternative Text)](https://semifive.com/wp-content/uploads/2022/04/ph_s5_logo_lrg.png "링크 설명(Title)은 생략 가능합니다.")

![대체 텍스트(Alternative Text)][Image참조링크]

[Image참조링크]: https://semifive.com/wp-content/uploads/2022/10/img_pkg_development_chip.jpg "이미지 설명은 생략할 수 있어요."
```
![대체 텍스트(Alternative Text)](https://semifive.com/wp-content/uploads/2022/04/ph_s5_logo_lrg.png "링크 설명(Title)은 생략 가능합니다.")

![대체 텍스트(Alternative Text)][Image참조링크]

[Image참조링크]: https://semifive.com/wp-content/uploads/2022/10/img_pkg_development_chip.jpg "이미지 설명은 생략할 수 있어요."

### Links
```
[GOOGLE](https://google.com)  
[NAVER](https://naver.com "링크 설명(title)은 생략할 수 있어요.")  
[AD팀][참조1]  

[참조1]: https://semifive.sharepoint.com/sites/Teams_AnalogDesign/Shared%20Documents  
[참조 링크]: https://naver.com "AD팀 쉐어포인트 링크입니다."  

문서 안에서 [참조 링크]를 그대로 사용할 수도 있습니다.
```
[GOOGLE](https://google.com)  
[NAVER](https://naver.com "링크 설명(title)은 생략할 수 있어요.")  
[AD팀][참조1]  

[참조1]: https://semifive.sharepoint.com/sites/Teams_AnalogDesign/Shared%20Documents  
[참조 링크]: https://naver.com "AD팀 쉐어포인트 링크입니다."  

문서 안에서 [참조 링크]를 그대로 사용할 수도 있습니다.

### 이미지에 링크 추가
```
[![대체 텍스트(Alternative Text)](https://semifive.com/wp-content/uploads/2022/04/ph_s5_logo_lrg.png)](https://semifive.sharepoint.com/sites/Teams_AnalogDesign/Shared%20Documents)
```
[![대체 텍스트(Alternative Text)](https://semifive.com/wp-content/uploads/2022/04/ph_s5_logo_lrg.png)](https://semifive.sharepoint.com/sites/Teams_AnalogDesign/Shared%20Documents)

## 5. 코드

### Blocks of code
\`를 3번 이상 입력하고 언어(코드) 이름을 명시해, 코드 '블록(Block)'를 표현합니다.
코드 블록의 시작 \` 개수와 종료 \` 개수는 같아야 합니다.
<pre>
<code>
```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```
</code>
</pre>

```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```

<pre>
<code>
```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```
</code>
</pre>

```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```

### Inline code
```
강조할 코드를 ` 기호로 감싸 `인라인(InLine)` 코드를 표현합니다.
```
강조할 코드를 \` 기호로 감싸 `인라인(InLine)` 코드를 표현합니다.

## 6. 인용문(Quotation)
```
> 인용문 - 남의 말이나 글에서 직접 또는 간접으로 따온 문장.
> _(네이버 국어 사전)_

BREAK!

> 인용문을 작성하세요!
>> 중첩된 인용문(nested blockquote)을 만들 수 있습니다.
>>> 중중첩 인용문 1
>>> 중중첩 인용문 2
>>> 중중첩 인용문 3
```
> 인용문 - 남의 말이나 글에서 직접 또는 간접으로 따온 문장.
> _(네이버 국어 사전)_

BREAK!

> 인용문을 작성하세요!
>> 중첩된 인용문(nested blockquote)을 만들 수 있습니다.
>>> 중중첩 인용문 1
>>> 중중첩 인용문 2
>>> 중중첩 인용문 3

## 7. 표(Tables)
테이블 헤더를 구분하기 위해, 3개 이상의 -(hyphen/dash) 기호를 사용합니다.

테이블 헤더를 구분하며 :(Colons) 기호를 추가해 셀(열/칸) 안에 내용을 정렬할 수 있습니다.

`---, :---`: 좌측 정렬

`:---:`: 가운데 정렬

`---:`: 우측 정렬
```
| Left columns  | Right columns |
| ------------- |:-------------:|
| left foo      | right foo     |
| left bar      | right bar     |
| left baz      | right baz     |
```
| Left columns  | Right columns |
| ------------- |:-------------:|
| left foo      | right foo     |
| left bar      | right bar     |
| left baz      | right baz     |

## 8. 체크박스
```
- [x] 완료
- [ ] 미완료
```
- [x] 완료
- [ ] 미완료


## 9. 수평선
```
---

***
```
---

***


## 10. 줄바꿈
```
줄바꿈(Line Breaks)을 위해서는 문장 마지막에서 <br>태그를 직접 입력하거나,      <!--띄어쓰기 2번-->
문장 마지막에서 띄어쓰기를 2번 이상 입력합니다.<!--띄어쓰기 없음-->
플랫폼 자체에서 자동 줄바꿈을 지원하는 경우,<!--띄어쓰기 없음-->
 이러한 방식이 필요하지 않을 수 있습니다.     <!--띄어쓰기 2번-->
Github에서는 줄바꿈을 위해 띄어쓰기를 2번이상 입력해야합니다.
```
줄바꿈(Line Breaks)을 위해서는 문장 마지막에서 <br>태그를 직접 입력하거나,   
문장 마지막에서 띄어쓰기를 2번 이상 입력합니다.
플랫폼 자체에서 자동 줄바꿈을 지원하는 경우, 이러한 방식이 필요하지 않을 수 있습니다.  
Github에서는 줄바꿈을 위해 띄어쓰기를 2번이상 입력해야합니다.

## 11. 주석
`<!-- -->`, `[//]: #` 기호를 사용해, 주석(Comment)을 표현합니다.
```
MARKDOWN
-- 시작 --

<!-- 안녕하세요. -->
[//]: # (안녕하세요.)
[//]: # "안녕하세요."
[//]: # '안녕하세요.'

-- 종료 --
```

-- 시작 --

-- 종료 --
