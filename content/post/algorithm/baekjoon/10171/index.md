---
author: 이승호
title: 고양이
description: "난이도: 브론즈 V"
date: 2023-02-23
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 고양이 www.acmicpc.net/problem/10171"
---

## 원글
> https://www.acmicpc.net/problem/10171

## 문제

> 아래 예제와 같이 고양이를 출력하시오.

### 입력

> 없음.

### 출력

> 고양이를 출력한다.

### 예제

#### 예제 출력 1

```
\    /\
 )  ( ')
(  /  )
 \(__)|
```

## 문제 풀이

### c++
```c++
#include <iostream>

using namespace std;

int main()
{
    // 출력
    cout << "\\    /\\" << "\n";
    cout << " )  ( ') "  << "\n";
    cout << "(  /  )"  << "\n";
    cout << " \\(__)|" << "\n";

    return 0;
}
```