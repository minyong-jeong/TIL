# 리스트 (List)

리스트란 순서대로 정리된 항목을 담는 자료형이다.

## 1) 리스트 선언

```python
>>> list = ["apple", "banana", "melon", "grape"]
>>> list
['apple', 'banana', 'melon', 'grape']
```

## 2) 리스트의 정렬, 삽입, 삭제, 수정

* sort()를 이용한 정렬

    ```python
    >>> list.sort()
    >>> list
    ['apple', 'banana', 'grape', 'melon']
    ```

* append()를 이용한 삽입

    ```python
    >>> list.append("mango")
    >>> list
    ['apple', 'banana', 'grape', 'melon', 'mango']
    ```

* del을 이용한 삭제

    ```python
    >>> del list[0]
    >>> list
    ['banana', 'grape', 'melon', 'mango']
    ```

* 수정

    직접 리스트의 값에 접근하여 값을 수정할 수 있다.

    ```python
    >>> list[0] = "pineapple"
    >>> list
    ['pineapple', 'grape', 'melon', 'mango']
    ```

