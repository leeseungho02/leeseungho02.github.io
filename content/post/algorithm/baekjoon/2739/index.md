---
author: 이승호
title: 구구단
description: "난이도: 브론즈 V"
date: 2023-02-22
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 구구단 www.acmicpc.net/problem/2739"
---

## 원글
> https://www.acmicpc.net/problem/2739

## 문제

> N을 입력받은 뒤, 구구단 N단을 출력하는 프로그램을 작성하시오. 출력 형식에 맞춰서 출력하면 된다.

### 입력

> 첫째 줄에 N이 주어진다. N은 1보다 크거나 같고, 9보다 작거나 같다.

### 출력

> 출력형식과 같게 N\*1부터 N\*9까지 출력한다.

### 예제

#### 예제 입력 1

> 2

#### 예제 출력 1

```
2 * 1 = 2
2 * 2 = 4
2 * 3 = 6
2 * 4 = 8
2 * 5 = 10
2 * 6 = 12
2 * 7 = 14
2 * 8 = 16
2 * 9 = 18
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
    for (int i = 1; i <= 9; i++) {
        cout << N << " * " << i << " = " << (N*i) << "\n";
    }
    
    return 0;
}
```