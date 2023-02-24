---
author: 이승호
title: 개
description: "난이도: 브론즈 V"
date: 2023-02-23
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 개 www.acmicpc.net/problem/10172"
---

## 원글
> https://www.acmicpc.net/problem/10172

## 문제

> 아래 예제와 같이 개를 출력하시오.

### 입력

> 없음.

### 출력

> 개를 출력한다.

### 예제

#### 예제 출력 1

```
|\_/|
|q p|   /}
( 0 )"""\
|"^"`    |
||_/=\\__|
```

## 문제 풀이

### c++
```c++
#include <iostream>

using namespace std;

int main()
{
    // 출력
    cout << "|\\_/|" << "\n";
    cout << "|q p|   /}" << "\n";
    cout << "( 0 )\"\"\"\\" << "\n";
    cout << "|\"^\"`    |" << "\n";
    cout << "||_/=\\\\__|" << "\n";

    return 0;
}
```