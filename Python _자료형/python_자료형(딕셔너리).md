# 딕셔너리 (Dictionary)

딕셔너리는 대응관계를 가지는 자료형이다. 전화번호부를 예로 들 수 있는데 누군가의 이름을 찾으면 그 이름에 대응되는 전화번호를 찾을 수 있는 것과 같다. 여기서 이름은 딕셔너리의 key가 되고, 전화번호는 value가 된다.

## 1) 딕셔너리의 선언

```python
>>> dic = {
... 'name':'kildong',
... 'email':'python@python.com',
... 'phone':'010-0000-0000'
... }
>>> dic
{'name': 'kildong', 'email': 'python@python.com', 'phone': '010-0000-0000'}
```

각각의 key에 대응하는 value값을 가진다. 여기서 key인 'name'에 대응하는 value는 'kildong'이다.

## 2) 딕셔너리 추가, 삭제

* 딕셔너리 추가

    ```python
    >>> dic['gender'] = 'male'
    >>> dic
    {'name': 'kildong', 'email': 'python@python.com', 'phone': '010-0000-0000', 'gender': 'male'}
    ```

* 딕셔너리 삭제

    ```python
    >>> del dic['phone']
    >>> dic
    {'name': 'kildong', 'email': 'python@python.com', 'gender': 'male'}
    ```

## 3) 딕셔너리에서 키 얻기

```python
>>> dic['name']
'kildong'
```
