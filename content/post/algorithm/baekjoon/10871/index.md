---
author: 이승호
title: X보다 작은 수
description: "난이도: 브론즈 V"
date: 2023-02-23
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 X보다 작은 수 www.acmicpc.net/problem/10871"
---

## 원글
> https://www.acmicpc.net/problem/10871

## 문제

> 정수 N개로 이루어진 수열 A와 정수 X가 주어진다. 이때, A에서 X보다 작은 수를 모두 출력하는 프로그램을 작성하시오.

### 입력

> 첫째 줄에 N과 X가 주어진다. (1 ≤ N, X ≤ 10,000)
> 
> 둘째 줄에 수열 A를 이루는 정수 N개가 주어진다. 주어지는 정수는 모두 1보다 크거나 같고, 10,000보다 작거나 같은 정수이다.

### 출력

> X보다 작은 수를 입력받은 순서대로 공백으로 구분해 출력한다. X보다 작은 수는 적어도 하나 존재한다.

### 예제

#### 예제 입력 1

```
10 5
1 10 4 9 2 3 8 5 7 6
```

#### 예제 출력 1

```
1 4 2 3
```

## 문제 풀이

### c++
```c++
#include <iostream>

using namespace std;

int main()
{
    // 첫째 줄 변수 선언
    int N, X;
    
    // 첫째 줄 입력
    cin >> N >> X;

    // 둘째 줄 변수 선언
    int A[N];

    // 둘째 줄 입력
    for (int i = 0; i < N; i++) {
        cin >> A[i];
    }

    // X보다 작은 수 출력
    for (int i = 0; i < (sizeof(A)/sizeof(*A)); i++) {
        if (X > A[i]) {
            cout << A[i] << " ";
        }
    }

    return 0;
}
```