---
author: 이승호
title: 별 찍기 - 2
description: "난이도: 브론즈 IV"
date: 2023-02-24
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 별 찍기 - 2 www.acmicpc.net/problem/2439"
---

## 원글
> https://www.acmicpc.net/problem/2439

## 문제

> 첫째 줄에는 별 1개, 둘째 줄에는 별 2개, N번째 줄에는 별 N개를 찍는 문제
> 
> 하지만, 오른쪽을 기준으로 정렬한 별(예제 참고)을 출력하시오.

### 입력

> 첫째 줄에 N(1 ≤ N ≤ 100)이 주어진다.

### 출력

> 첫째 줄부터 N번째 줄까지 차례대로 별을 출력한다.

### 예제

#### 예제 입력 1

```
5
```

#### 예제 출력 1

```
    *
   **
  ***
 ****
*****
```

## 문제 풀이

### c++
```c++
#include <iostream>

using namespace std;

int main()
{
    // 변수 선언
    int N;

    // 입력
    cin >> N;

    // 출력
    for (int i = 0; i < N; i++) {
        for (int j = (N - i); j > 1; j--) {
            cout << " ";
        }
        for (int j = 0; j <= i; j++) {
            cout << "*";
        }
        cout << "\n";
    }

    return 0;
}
```