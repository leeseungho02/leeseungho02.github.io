---
author: 이승호
title: 기찍 N
description: "난이도: 브론즈 IV"
date: 2023-02-24
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 기찍 N www.acmicpc.net/problem/2742"
---

## 원글
> https://www.acmicpc.net/problem/2742

## 문제

> 자연수 N이 주어졌을 때, N부터 1까지 한 줄에 하나씩 출력하는 프로그램을 작성하시오.

### 입력

> 첫째 줄에 100,000보다 작거나 같은 자연수 N이 주어진다.

### 출력

> 첫째 줄부터 N번째 줄 까지 차례대로 출력한다.

### 예제

#### 예제 입력 1

```
5
```

#### 예제 출력 1

```
5
4
3
2
1
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