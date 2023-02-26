---
author: 이승호
title: 숫자의 개수
description: "난이도: 브론즈 II"
date: 2023-02-25
categories: [
    "알고리즘-백준",
]
keywords: "알고리즘 백준 숫자의 개수 www.acmicpc.net/problem/2577"
---

## 원글
> https://www.acmicpc.net/problem/2577

## 문제

> 세 개의 자연수 A, B, C가 주어질 때 A × B × C를 계산한 결과에 0부터 9까지 각각의 숫자가 몇 번씩 쓰였는지를 구하는 프로그램을 작성하시오.
> 
> 예를 들어 A = 150, B = 266, C = 427 이라면 A × B × C = 150 × 266 × 427 = 17037300 이 되고, 계산한 결과 17037300 에는 0이 3번, 1이 1번, 3이 2번, 7이 2번 쓰였다.

### 입력

> 첫째 줄에 A, 둘째 줄에 B, 셋째 줄에 C가 주어진다. A, B, C는 모두 100보다 크거나 같고, 1,000보다 작은 자연수이다.

### 출력

> 첫째 줄에는 A × B × C의 결과에 0 이 몇 번 쓰였는지 출력한다. 마찬가지로 둘째 줄부터 열 번째 줄까지 A × B × C의 결과에 1부터 9까지의 숫자가 각각 몇 번 쓰였는지 차례로 한 줄에 하나씩 출력한다.

### 예제

#### 예제 입력 1

```
150
266
427
```

#### 예제 출력 1

```
3
1
0
2
0
0
0
2
0
0
```

## 문제 풀이

### c++
```c++
#include <iostream>

using namespace std;

int main()
{
    // 변수 선언
    int A, B, C;
    
    // 입력
    cin >> A >> B >> C;
    
    // 구현
    string result = to_string(A * B * C);
    int use_number_count[10] = {0, 0, 0, 0, 0, 0, 0, 0, 0, 0};
    char check_number_list[10] = {'0', '1', '2', '3', '4', '5', '6', '7', '8', '9'};
    for (int i = 0; i < result.size(); i++) {
        for (int j = 0; j <= 9; j++) {
           if (result[i] == check_number_list[j]) {
                use_number_count[j]++;
            }
        }
    }
    
    // 출력
    for (int i = 0; i < sizeof(use_number_count)/sizeof(int); i++) {
        cout << use_number_count[i] << "\n";
    }
    
    return 0;
}
```