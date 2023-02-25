---
author: 이승호
title: 숫자의 합
description: "난이도: 브론즈 IV"
date: 2023-02-24
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 숫자의 합 www.acmicpc.net/problem/11720"
---

## 원글
> https://www.acmicpc.net/problem/11720

## 문제

> N개의 숫자가 공백 없이 쓰여있다. 이 숫자를 모두 합해서 출력하는 프로그램을 작성하시오.

### 입력

> 첫째 줄에 숫자의 개수 N (1 ≤ N ≤ 100)이 주어진다. 둘째 줄에 숫자 N개가 공백없이 주어진다.

### 출력

> 입력으로 주어진 숫자 N개의 합을 출력한다.

### 예제

#### 예제 입력 1

```
1
1
```

#### 예제 출력 1

```
1
```

#### 예제 입력 2

```
5
54321
```

#### 예제 출력 2

```
15
```

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
    string number;
    // 둘째 줄 입력
    cin >> number;
    
    // 구현
    int sum = 0;
    for (int i = 0; i < N; i++) {
        sum += number[i] - '0';
    }
    
    // 출력
    cout << sum;
    
    return 0;
}
```