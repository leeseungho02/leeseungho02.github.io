---
author: 이승호
title: A / B
description: "난이도: 브론즈 V"
date: 2023-02-22
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 A/B www.acmicpc.net/problem/1008"
---

## 원글
> https://www.acmicpc.net/problem/1008

## 문제
> 두 정수 A와 B를 입력받은 다음, A/B를 출력하는 프로그램을 작성하시오.

### 입력

> 첫째 줄에 A와 B가 주어진다. (0 < A, B < 10)

### 출력

> 첫째 줄에 A/B를 출력한다. 실제 정답과 출력값의 절대오차 또는 상대오차가 10-9 이하이면 정답이다.

### 예제

#### 예제 입력 1

> 1 3

#### 예제 출력 1

> 0.33333333333333333333333333333333
 
#### 예제 입력 2

> 4 5

#### 예제 출력 2

> 0.8

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
    
    // 답 1안
    printf("%.12f", (double)A/(double)B);

    // 답 2안
    cout << fixed;
    cout.precision(12);
    cout << (double)A/(double)B << endl;
    cout.unsetf(ios::fixed);
    
    return 0;
}
```