[Git특강](https://hphk.notion.site/hphk/Git-21-12-21-21-12-22-2c1e3a19b113452e815b237c507704b9) 

## CLI

- GUI (Graphic User Interface): 

  그래픽을 통해 사용자와 컴퓨터가 상호 작용하는 방식

- CLI (Command Line Interface): 

  터미널을 통해 사용자와 컴퓨터가 상호 작용하는 방식

### [1] 경로

#### (0) 루트 디렉토리 '/'

- 모든 파일과 폴더를 담고 있는 최상위 폴더

#### (1) 홈 디렉토리 '~'

- 현재 로그인 된 사용자의 홈 폴더 
  - e.g. `/Users/사용자계정` 

#### (2) 절대경로

- 루트 디렉토리부터 목적 지점까지 거치는 모든 경로 
  - e.g. `/Users/sujiyang/Desktop`

#### (3) 상대경로

- 현재 작업 중인 디렉토리를 기준으로 상대적 위치
  - `.` 나 자신
  - `..` 부모
    - `./` 현재 작업 중인 폴더
    - `../` 현재 작업 중인 폴더의 부모 폴더

### [2] 터미널

#### (0) 유용한 단축키

- 위, 아래 방향키: 썼던 커맨드 재사용
- tab` : 폴더/파일 이름 자동완성
- `ctrl+l` : 화면 맨 밑단으로 내려가기

#### (1) 명령어

1. `open`

- (mac) 폴더/파일 열어주세요. 

```python
# 현재 작업 중인 위치 열어주세요
$ open . # mac
$ start . # windows
```

2. `pwd`

- print working directory
- 현재 작업 경로를 보여주세요.

3.  `mkdir` ..

- make directory
- .. 폴더 만들어주세요
  - 폴더명 안에 공백을 포함시키려면 ' ' 사용
  - 띄어쓰기로 여러 폴더 한꺼번에 생성 가능

```python
$ mkdir folder
$ mkdir 'multi campus' 'fast campus'
```

4. `ls`

- list segments
- 현재 작업 중인 디렉토리의 목록 보여주세요
  - ls -a (all)   숨긴파일까지 보여주세요
  - ls -l (long)   자세하게 보여주세요

```python
# 기본 사용
$ ls
# all, long 옵션 띄어쓰기로 함께 적용 (순서 상관 없음)
$ ls -a -l
```

5. `cd` ..

- change directory
- ..으로 디렉토리를 변경해주세요

```python
# folder로 이동
$ cd folder

# 절대 경로
$ cd /Users/sujiyang/Desktop

# 상대 경로 
$ cd .			# 현재 작업 위치로 이동
$ cd ..			# 현재 작업 위치의 상위로 이동 (위로 가기)
$ cd - 			# 현재 작업 위치의 바로 전으로 이동 (뒤로 가기)
```

6. `touch` ..

- .. 파일 생성해주세요
  - 띄어쓰기로 여러파일 한꺼번에 생성 가능
  - 파일명 앞에 `.` 을 붙여서 숨김파일 생성

```python
$ touch file.txt
$ touch A.txt B.txt C.txt
```

7. `rm` ..

- remove
- .. 파일/폴더 지워주세요

```python
# 해당 파일 삭제
$ rm file.txt
# 해당 폴더 삭제
$ rm -r folder # (recursive) 폴더 삭제시 사용

# 모든 txt 확장자 파일 삭제
$ rm *.txt
```

8. `mv` .. ..

- move
  - 폴더/파일을 다른 폴더 내로 이동
  - 폴더/파일 이름을 변경

```python
# file.txt를 folder 안으로 이동
$ mv file.txt folder # folder라는 폴더가 존재해야

# 파일명 file.txt를 file1.txt로 변경
$ mv file.txt	file1.txt
```



## Markdown

#### (0) 마크다운이란?

- 텍스트기반의 경량 Markup 언어
- 마크업을 더 쉽고 간단하게 사용하고자 만들어짐
- .md 확장자를 가짐
- 마크다운의 본질은 글에게 역할을 부여하는 것에 있음!

#### (1) 문법

더 자세한 내용은 [GitHub Docs](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) 클릭해서 확인해보기

1. 제목 Headings

- `#` 을 사용해서 제목 표현

```python
# 제일 큰 제목
## 두번째로 큰 제목
### 세번째로 큰 제목
###### 가장 작은 제목
```

# 제목1

## 제목 2

### 제목3

#### 제목4

##### 제목5

###### 제목 6



2. 목록 Lists



3. 글자 스타일 Styling text

- 굵게                         `**글자** `     **이렇게**
- 기울이기                  `*글자*`         *이렇게*
- 취소                         `~~글자~~`     ~~이렇게~~
- 굵고 기울게 섞어서   `**다 굵고 _얘만_ 기울여서**`     **다 굴고 _얘만_  기울여서**
- 전부 굵고 기울게      `***전부 다 굵고 기울여서***`     ***전부 다 굵고 기울여서***



4. 인용 Quoting

- 텍스트 인용 `>`

```python
인용이 아닌 텍스트
> 인용인 텍스트
```

인용이 아닌 텍스트

>  인용인 텍스트

- 코드인용
  - inline 코드 - backtick 한개 `` ` ``
  - block 코드 - backtick 세개 ```

1. 표 Tables
2. 이미지 Images
3. 링크 Links
4. 마크다운 형식 무시 Escape













[Github Markdown](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

---



###### 

----

목록

순서가 없는 목록

- 목록1
- 목록2
- 목록3

슈퍼

- 과일
  - 참외
  - 수박

순서가 있는 목록

1. 목록 1
2. 목록 2
   1. 목록 2-1
   2. 목록 2-2
      1. 목록 2-2-1
      2. 목록 2-2-2

----

강조(스타일링)

1. 기울임(이탤릭체): *글자*
2. 굵게(볼드체): **글자**
3. 취소선: ~~글자~~

----

코드

인라인 코드(=한줄) -> 백틱 `

파이썬에는 `print("Hello World!")`라고 쓸 수 있습니다.



블록 코드(=여러줄)

```python
for i in range(10):
   print(i)
```

----

수평선

\--- 작성 후 엔터

----

표(테이블)

행 추가는 cntrl+enter

| 동물   | 다리개수 | 종     |
| ------ | -------- | ------ |
| 사자   | 4개      | 포유류 |
| 원숭이 | 2개      | 포유류 |
| 앵무새 | 2개      | 조류   |

----

