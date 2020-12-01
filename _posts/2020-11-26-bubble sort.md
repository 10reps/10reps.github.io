---
title: "버블정렬"
date: 2020-11-26
tags:
header:
  image: "/assets/images/code.jpg"
---

### 버블정렬

* 인접한 두개의 원소를 비교하여 자리를 교환하는 방식의 알고리즘이다.

* 시간복잡도 O(n²)

* 버블정렬 방법

<img src="{{ site.url }}{{ site.baseurl }}/assets/images/bubble.png" alt="">

* 버블정렬 알고리즘

```python
    def bubble(arr):
        bulen = len(arr) - 1
        for i in range(bulen):
            for j in range(bulen - i):
                if arr[j] > arr[j + 1]:
                    arr[j], arr[j + 1] = arr[j + 1], arr[j]
        return arr

    arr = list(map(int, input().split())) # 공백을 기준으로 데이터입력
    print(bubble(arr))
```