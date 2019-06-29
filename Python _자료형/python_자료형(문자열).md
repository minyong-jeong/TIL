# 문자열(String)

문자열은 문자들의 나열 다르게 말하면 문자들의 집합이다.

## 1) 문자열 표현 방식

### 작은 따옴표

```python
>>> str = 'Hello world!'
>>> str
'Hello world!'
```

### 큰 따옴표

```python
>>> str = "Hello world!"
>>> str
'Hello world!'
```

### 여러 줄의 문자열을 표현하고 싶을 때 (연속된 3개의 따옴표를 이용)

```python
>>> str = '''Hello
... world!
... hahaha'''
>>> str
'Hello\nworld!\nhahaha'
```

## 2) 문자열 연산

### 문자열 연결

+연산은 두개 또는 그 이상의 문자열을 연결해준다.

```python
>>> str1 = "Hello "
>>> str2 = "world!"
>>> str1 + str2
'Hello world!'
```

### 문자열 곱하기

*연산은 문자열을 반복하라는 의미이다.

```python
>>> str = "Hello"*3
>>> str
'HelloHelloHello'
```

## 3) 문자열 인덱싱과 슬라이싱

### 인덱싱 (Indexing)

인덱싱은 가리키다라는 의미를 가지고 있고, 위 예시에서 문자열에 3번째 위치한 문자는 h인 것을 알 수 있다. (0번 부터 순서를 센다.)

```python
>>> str = "Python nojam"
>>> str[3]
'h'
```

위치 값에 마이너스를 넣은 경우 뒤에서 부터 읽는다. (위 예제에서 뒤에서 2번째 값은 ‘l’)

```python
>>> str = "Example"
>>> str[-2]
'l'
```

### 슬라이싱 (Slicing)

인덱싱은 하나의 문자 값을 얻어낸다면 슬라이싱은 단어(여러개의 문자)를 얻어낼 수 있다.

0 ~ 2 번째에 해당하는 단어를 얻어낼 수 있다.

```python
>>> str = "Welcome to Helloworld!"
>>> str[0:3]
'Wel'
```

str[시작번호:끝번호]에서 시작번호 또는 끝 번호를 생략할 경우 생략한 부분 전부를 얻어낸다.

str[:]일 경우 문자열 전체를 반환한다.

```python
>>> str = "Welcome to Helloworld!"
>>> str[3:]
'come to Helloworld!'
>>> str[:10]
'Welcome to'
>>> str[:]
'Welcome to Helloworld!'
```

\- 연산자도 사용이 가능하다. str[10:-3]은 10번째 부터 -4까지 문자를 뜻한다.

```python
>>> str = "Welcome to Helloworld!"
>>> str[10:-3]
' Hellowor'
```

## 4) 문자열 포맷팅

문자열 포맷팅은 문자열 내에 어떤 단어나 숫자를 삽입하기 위해서 사용된다. 이를 위해서 format()이 사용된다.

숫자와 문자를 바로 대입할 수 있다.

```python
>>> "Hello {0}".format("world!")
'Hello world!'
>>> "Number {0}".format(5)
'Number 5'
```

또는 변수를 바로 대입할 수 있다.

```python
>>> insert = "dev"
>>> "Hello {0}".format(insert)
'Hello dev'
```

괄호 안의 숫자를 생략할 수도 있다.

```python
>>> str1 = "X"
>>> str2 = "Y"
>>> "{} + {}".format(str1, str2)
'X + Y'
```
