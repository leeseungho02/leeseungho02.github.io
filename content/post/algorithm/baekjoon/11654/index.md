---
author: 이승호
title: 아스키 코드
description: "난이도: 브론즈 V"
date: 2023-02-23
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 아스키 코드 www.acmicpc.net/problem/11654"
---

## 원글
> https://www.acmicpc.net/problem/11654

## 문제

> 알파벳 소문자, 대문자, 숫자 0-9중 하나가 주어졌을 때, 주어진 글자의 아스키 코드값을 출력하는 프로그램을 작성하시오.

### 입력

> 알파벳 소문자, 대문자, 숫자 0-9 중 하나가 첫째 줄에 주어진다.

### 출력

> 입력으로 주어진 글자의 아스키 코드 값을 출력한다.

### 예제

#### 예제 입력 1

```
A
```

#### 예제 출력 1

```
65
```

#### 예제 입력 2

```
0
```

#### 예제 출력 2

```
48
```

## 문제 풀이

### c++
```c++
#include <iostream>

using namespace std;

int main()
{
    // 변수 선언
    char word;

    // 입력
    cin >> word;

    // 출력 - 답 1안
    cout << (int) word;

    // 출력 - 답 2안
    cout << static_cast<int>(word);

    return 0;
}
```