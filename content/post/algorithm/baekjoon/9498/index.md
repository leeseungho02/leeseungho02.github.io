---
author: 이승호
title: 시험 성적
description: "난이도: 브론즈 V"
date: 2023-02-23
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 시험 성적 www.acmicpc.net/problem/9498"
---

## 원글
> https://www.acmicpc.net/problem/9498

## 문제

> 시험 점수를 입력받아 90 ~ 100점은 A, 80 ~ 89점은 B, 70 ~ 79점은 C, 60 ~ 69점은 D, 나머지 점수는 F를 출력하는 프로그램을 작성하시오.

### 입력

> 첫째 줄에 시험 점수가 주어진다. 시험 점수는 0보다 크거나 같고, 100보다 작거나 같은 정수이다.

### 출력

> 시험 성적을 출력한다.

### 예제

#### 예제 입력 1

> 100

#### 예제 출력 1

> A

## 문제 풀이

### c++
```c++
#include <iostream>

using namespace std;

int main()
{
    // 변수 선언
    int score;
    
    // 입력
    cin >> score;
    
    // 출력
    if (score >= 90 && score <= 100) {
        cout << "A";
    } else if (score >= 80 && score <= 89) {
        cout << "B";
    } else if (score >= 70 && score <= 79) {
        cout << "C";
    } else if (score >= 60 && score <= 69) {
        cout << "D";
    } else {
        cout << "F";
    }
    
    return 0;
}
```