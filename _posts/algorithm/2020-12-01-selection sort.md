---
title: "Selection sort"
date: 2020-12-01
tags:
header:
  image: "/assets/images/code.jpg"
excerpt: "Algorithm"
---

### 선택정렬

* 처리할 데이터 범위에서 최솟값을 찾아 그 값과 데이터 맨 앞의 값을 비교 후 자리를 바꾸는 과정이다.

* 시간복잡도 O(n²)

* 선택정렬 방법

<img src="{{ site.url }}{{ site.baseurl }}/assets/images/Algorithm/selection.png" alt="">

* 선택정렬 알고리즘

```python
    def selection(arr):
        for i in range(len(arr) - 1):
            min_value = i
            for j in range(i + 1, len(arr)):
                if arr[min_value] > arr[j]:
                    min_value = j
            arr[i], arr[min_value] = arr[min_value], arr[i]

        return arr
    
    arr = list(map(int, input().split()))
    print(selection(arr))
```