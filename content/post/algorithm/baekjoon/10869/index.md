---
author: 이승호
title: 사칙연산
description: "난이도: 브론즈 V"
date: 2023-02-23
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 사칙연산 www.acmicpc.net/problem/10869"
---

## 원글
> https://www.acmicpc.net/problem/10869

## 문제

> 두 자연수 A와 B가 주어진다. 이때, A+B, A-B, A*B, A/B(몫), A%B(나머지)를 출력하는 프로그램을 작성하시오. 

### 입력

> 두 자연수 A와 B가 주어진다. (1 ≤ A, B ≤ 10,000)

### 출력

> 첫째 줄에 A+B, 둘째 줄에 A-B, 셋째 줄에 A*B, 넷째 줄에 A/B, 다섯째 줄에 A%B를 출력한다.

### 예제

#### 예제 입력 1

> 7 3

#### 예제 출력 1

```
10
4
21
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
    int A, B;
    
    // 입력
    cin >> A >> B;
    
    // 출력
    cout << (A+B) << "\n";
    cout << (A-B) << "\n";
    cout << (A*B) << "\n";
    cout << (A/B) << "\n";
    cout << (A%B) << "\n";

    return 0;
}
```