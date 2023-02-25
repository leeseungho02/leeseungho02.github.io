---
author: 이승호
title: 최소, 최대
description: "난이도: 브론즈 III"
date: 2023-02-24
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 최소, 최대 www.acmicpc.net/problem/10818"
---

## 원글
> https://www.acmicpc.net/problem/10818

## 문제

> N개의 정수가 주어진다. 이때, 최솟값과 최댓값을 구하는 프로그램을 작성하시오.

### 입력

> 첫째 줄에 정수의 개수 N (1 ≤ N ≤ 1,000,000)이 주어진다. 둘째 줄에는 N개의 정수를 공백으로 구분해서 주어진다. 모든 정수는 -1,000,000보다 크거나 같고, 1,000,000보다 작거나 같은 정수이다.

### 출력

> 첫째 줄에 주어진 정수 N개의 최솟값과 최댓값을 공백으로 구분해 출력한다.

### 예제

#### 예제 입력 1

```
5
20 10 35 30 7
```

#### 예제 출력 1

> 7 35

## 문제 풀이

### c++
```c++
#include <iostream>

using namespace std;

int main()
{
    // 첫째 줄 변수 선언
    int N;
    
    // 첫째 줄 입력
    cin >> N;
    
    // 둘째 줄 변수 선언
    int number[N];
    for (int i = 0; i < N; i++) {
        cin >> number[i];
    }
    
    // 구현
    int max = number[0];
    int min = number[0];
    for (int i = 0; i < (sizeof(number) / sizeof(int)); i++) {
        if (number[i] > max) {
            max = number[i];
        }
        if (number[i] < min) {
            min = number[i];
        }
    }
    
    // 출력
    cout << min << " " << max;
    
    return 0;
}
```