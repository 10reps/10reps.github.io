---
title: "이진탐색"
date: 2020-11-19
tags:
header:
  image: "/assets/images/code.jpg"
---
배경

<img src="{{ site.url }}{{ site.baseurl }}/assets/images/money1.jpg" alt="">

A는 9300원이 들어있는 상자를 찾고싶다.

선형탐색
순차적으로 차례대로 탐색(정리되어있지 않은 자료탐색시 유리)
정리되어있지 않은 자료라도 사용가능한 방법

```python
    i = [10, 200, 700, 1100, 4300, 6900, 9300, 13200, 34000, 50000]
    j = int(input('찾는 숫자를 입력하세요: '))

    for k in range(len(i)+1):
        if i[k] == j:
            print('%d는 %d번 인덱스에 있습니다.' % (j, k))
            break
``

이진탐색
정리되어있는 데이터를 탐색할때 사용가능하고 정리되어있지 않으면 불가능한 방법
