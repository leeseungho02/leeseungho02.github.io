---
author: 이승호
title: A+B - 5
description: "난이도: 브론즈 V"
date: 2023-02-23
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 A+B - 5 www.acmicpc.net/problem/10952"
---

## 원글
> https://www.acmicpc.net/problem/10952

## 문제

> 두 정수 A와 B를 입력받은 다음, A+B를 출력하는 프로그램을 작성하시오.

### 입력

> 입력은 여러 개의 테스트 케이스로 이루어져 있다.
>
> 각 테스트 케이스는 한 줄로 이루어져 있으며, 각 줄에 A와 B가 주어진다. (0 < A, B < 10)
>
> 입력의 마지막에는 0 두 개가 들어온다.

### 출력

> 각 테스트 케이스마다 A+B를 출력한다.

### 예제

#### 예제 입력 1

```
1 1
2 3
3 4
9 8
5 2
0 0
```

#### 예제 출력 1

```
2
5
7
17
7
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
    while (cin >> A >> B) {
        // 입력 마지막 0 두개 체크 조건
        if (A == 0 && B == 0) {
            break;
        }
        // 출력
        cout << (A+B) << "\n";
    }

    return 0;
}
```