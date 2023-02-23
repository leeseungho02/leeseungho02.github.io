---
author: 이승호
title: N 찍기
description: "난이도: 브론즈 V"
date: 2023-02-22
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 N 찍기 www.acmicpc.net/problem/2741"
---

## 원글
> https://www.acmicpc.net/problem/2741

## 문제

> 자연수 N이 주어졌을 때, 1부터 N까지 한 줄에 하나씩 출력하는 프로그램을 작성하시오.

### 입력

> 첫째 줄에 100,000보다 작거나 같은 자연수 N이 주어진다.

### 출력

> 첫째 줄부터 N번째 줄 까지 차례대로 출력한다.

### 예제

#### 예제 입력 1

> 5

#### 예제 출력 1

```
1
2
3
4
5
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
    for (int i = 1; i <= N; i++) {
        cout << i << "\n";
    }
    
    return 0;
}
```