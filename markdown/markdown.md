# amrkdown 기초 문법

---

## 리스트 (ordered list)
1. 손 씻기
   1. 손을 뻗고
   2. 물을 틀어서
   3. 손을 씻는다.
2. 식당에 가기

---

## 인라인 강조
중요한 것은 **굵게** 표시하고, 주의할 것은 *기울이고*, `코드 혹은 명령어(빽틱)`는 따로 표시를 하고 싶다.
- 굵게 할 떄는 * 두 개로 감싼다. (**bold**)
- 이탤릭체는 * 한 개로 감싼다. (*italic*)
- 코드 강조는 \` 두개로 감싼다. (`code`)

variables may be found in `setup.py`

---

## 블럭 강조
### 표
파이프( | )로 구분하여 테이블 헤더를 생성한다.

* 표 만들기 (table)

|명령어|설명|예시|
|-|-|-|
|`$`|터미널에 명령어 입력 준비가 되어 있다는 의미|
|`mkdir`|폴더를 생성한다.|`$ mkdir my_dir`|
|`touch`|파일을 생성한다.|`$ touch a.txt` |
|`rm`|파일을 삭제한다.|`$ rm a.txt` |
|`rm -r`|폴더를 삭제한다.|`$ rm -r my_dir` |
|`ls`|현재 위치 폴더의 모든 하위 항목 표시|`$ ls` |
|`cd`|디렉토리 경로 변경|`$ cd cli` |
|`cd ..`|상위 디렉토리로 이동|`$ cd ..` |
|`cd ~`|홈 디렉토리로 이동|`$ cd ~`|
|`code .`|폴더를 vscode에서 열기|`$ code .` |
|`ctrl + l`|터미널 정리(c`l`ear)|
|`ctrl + c`|취소(`c`ancle), 터미널 프롬프트가 `>`로 바꼈을 때 다시 `$`바꾸기|
|`ctrl + p` + `> select default ~` + `git bash`|vscode에서 터미널 변경|
|`ctrl + `\`|vscode에서 터미널 올리기|
|`/`|최상단(root) 폴더 상징 기호|`& cd /`|
|`cd .`|현재 위치 상징 기호|`$ cd .`|


### 코드
아래와 같이 진행된다.

```
$ mkdir mydir
$ cd mydir
$ touch a.txt
```

```
# python
def my_func(x, y):
    return x + y
```

```python
# python
def my_func(x, y):
    return x + y
```
---

## 기타

### 인용문

> 일단 유명해 져라. - 유태영

### 수식
- 인라인 수식: $x + y$
- 블럭 수식
$$
\mathbb{N}=\{a\in\mathbb{Z}:a>0\}
$$

### 이미지 / 하이퍼링크
```
\syntax: [표시 텍스트](링크)
```

[구글](https://google.com)

```
image
\syntax: ![대체 텍스트](링크)
```
