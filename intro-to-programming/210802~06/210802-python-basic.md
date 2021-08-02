# Python

## Python

Python은 1991년에 발표된, 인터프리터 방식의 프로그래밍 언어이다.


## Python의 장점과 단점

### 장점

작성한 코드를 실행가능한 프로그램으로 만들 필요가 없음
스크립트를 실행해줄 프로그램만 설치하면 어디든 실행가능


### 단점

성능이 느림




## Python 변수의 종류

숫자형: 정수, 실수 등의 숫자를 다루는 자료형 


문자열: 문자열을 다루는 자료형 ‘ ’, “ ” 사용


리스트: 다른 자료형의 모음을 다루는 자료형(배열과 같이 생각중)


튜플: 리스트와 같지만 수정이 불가능한 자료형


딕셔너리: 키와 값으로 이루어진 자료형 {‘key’ : ‘value’}





## Python 문자열 - 내장함수


count : 특정 문자 수를 반환

```
v = ‘value’

result = v.count(‘v’)

result의 값 = 2
```

find: 특정 문자 위치를 반환

```
v = ‘value’

result = v.count(‘v’)

result의 값 = 2
```

replace: 문자열을 치환한 결과 반환

```
v = ‘Goodvalue’

result = v.replace(‘Good’, ‘Bad’)

result의 값 = Badvalue
```


## Python 리스트 - 내장함수

append: 요소를 뒤에 추가

```
result = [1,2,3]

result.append(4)

result의 값 = [1,2,3,4]
```

sort: 요소들을 정렬

```
result = [‘a’, ‘b’, ‘c’]

result.sort()

result의 값 = [‘a’, ‘b’, ‘c’]
```

reverse: 요소들을 뒤집음

```
result = [1, 10, 100]

result.reverse()

result의 값 = [100, 10, 1]
```


index: 입력값의 위치를 반환

```
result = [10, 11, 11, 100]

result.index(11)

result의 값 = 1
```

insert: 특정 위치에 요소를 추가

```
result = [100, 192, 101]

result.insert(1,’a’)

result의 값 = [100, ‘a’, 192, 101 ]
```

remove: 입력값을 삭제

```
result = [10, 11, 100, 11]

result.remove(11)

result의 값 = [10, 100, 11]
```

pop: 마지막 요소를 꺼내고 삭제

```
a = [10, 101, 102, 103]

result = a.pop()

result의 값 = 103
```


## Python 딕셔너리 - 내장함수


keys: 딕셔너리의 key들을 반환

```
a = {‘a’ : 123, ‘b’ : 456}

result = a.keys()

result의 값 =  dict_keys([‘a’, ‘b’])
```

values: 딕셔너리의 value들을 반환

```
a = {‘a’ : 123, ‘b’ : 456}

result = a.values()

result의 값 =  dict_values([123, 456])
```

items: key, value 쌍을 반환

```
a = {‘a’ : 123}

result = a.items()

result의 값 =  dict_items([‘a’, 123])
```


## Python의 조건문

### 문법


```
if 조건문:

    실행할 문장



elif 조건문:

    실행할 문장



else:

    실행할 문장

```

주의점: 공백은 tab, space 전부 다 가능하지만 꼭 같은 공백 사용





## Python의 반복문(for문)

### 문법


```
for 변수명 in 리스트, 튜플, 문자열:

    실행할 문장
    실행할 문장



```

range 함수: range 함수는 입력한 숫자에 맞는 리스트를 만들어 줌

for looper in range(100):
    print(looper)

결과: 0~99 까지 출력


## Python의 반복문(while문)

### 문법

```
while 조건문:

    실행할 문장


주의점: 특정 조건이 만족할 때 까지 계속 반복

```

break, continue
break: 반복문에서 빠져 나오는 구문
continue: 반복문에서 뒤 문장을 건너뛰는 구문


