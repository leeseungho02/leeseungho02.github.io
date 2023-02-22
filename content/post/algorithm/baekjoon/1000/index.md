---
author: 이승호
title: A + B
description: "난이도: 브론즈 V"
date: 2023-02-22
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 A+B www.acmicpc.net/problem/1000"
---

## 원글
> https://www.acmicpc.net/problem/1000

## 문제
> 두 정수 A와 B를 입력받은 다음, A+B를 출력하는 프로그램을 작성하시오.

### 입력

> 첫째 줄에 A와 B가 주어진다. (0 < A, B < 10)

### 출력

> 첫째 줄에 A+B를 출력한다.

### 예제

#### 예제 입력 1

> 1 2

#### 예제 출력 1

> 3

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
    cout << (A+B);
    
    return 0;
}
```