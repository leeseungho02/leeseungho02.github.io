---
author: 이승호
title: 문자열 반복
description: "난이도: 브론즈 II"
date: 2023-02-25
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 문자열 반복 www.acmicpc.net/problem/2675"
---

## 원글
> https://www.acmicpc.net/problem/2675

## 문제

> 문자열 S를 입력받은 후에, 각 문자를 R번 반복해 새 문자열 P를 만든 후 출력하는 프로그램을 작성하시오. 즉, 첫 번째 문자를 R번 반복하고, 두 번째 문자를 R번 반복하는 식으로 P를 만들면 된다. S에는 QR Code "alphanumeric" 문자만 들어있다.
> 
> QR Code "alphanumeric" 문자는 0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ\$%*+-./: 이다.

### 입력

> 첫째 줄에 테스트 케이스의 개수 T(1 ≤ T ≤ 1,000)가 주어진다. 각 테스트 케이스는 반복 횟수 R(1 ≤ R ≤ 8), 문자열 S가 공백으로 구분되어 주어진다. S의 길이는 적어도 1이며, 20글자를 넘지 않는다.

### 출력

> 각 테스트 케이스에 대해 P를 출력한다.

### 예제

#### 예제 입력 1

```
2
3 ABC
5 /HTP
```

#### 예제 출력 1

```
AAABBBCCC
/////HHHHHTTTTTPPPPP
```

## 문제 풀이

### c++
```c++
#include <iostream>

using namespace std;

int main()
{
    // 첫째 줄 변수 선언
    int T;
    
    // 첫째 줄 입력
    cin >> T;
    
    // 둘째 줄 변수 선언
    int R;
    string S;
    
    // 데스트 케이스 만큼 입력 받기
    for (int i = 0; i < T; i++) {
        // 둘째 줄 입력
        cin >> R >> S;
        
        // 문자열 만큼 반복
        for (int j = 0; j < S.length(); j++) {
            // 문자열 내 문자를 R번 만큼 반복해서 출력
            for (int k = 0; k < R; k++) {
                cout << S[j];
            }
        }
        cout << "\n";
    }
    
    return 0;
}
```