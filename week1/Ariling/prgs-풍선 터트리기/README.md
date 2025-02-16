# 🔎 풍선 터트리기

https://school.programmers.co.kr/learn/courses/30/lessons/68646

## 💡 아이디어

- 구현 문제로 0부터 끝까지 idx를 기준으로 전, 후 최소값들을 구하여 처리를 하면 된다.

## ✔ 문제풀이

> **python && js**

- a의 인덱스를 기준으로 전, 후 구간들의 최소값을 담아둔다.
- 후 구간의 경우에는 reverse()를 활용하여 뒤집는다.
- 그 뒤 둘 다 큰 경우에는 최후까지 남을 수 없으므로 그 이외의 경우만 += 1 처리를 한다.

## 🤕 어려웠던 점

- 시간초과가 어려웠던 문제... 어떻게 시간초과를 안 내고 구현하는지가 관건이었다.
  - 처음에는 idx마다 전, 후 구간들을 최소값을 구해서 시간초과가 일어났다. 이 문제는 O(N^2)이 나오면 안 됐던 것
  - 2,3차는 미리 담아뒀음에도 appendleft를 하든 0번 인덱스에 append를 하든 O(N)이 아니므로 시간초과가 일어났다...
    - 이는 js의 unshift도 마찬가지! 앞자리에 넣는 메소드들은 reverse를 이길 수 없나보다..
  - 마지막에 배열을 뒤집는 메서드인 reverse를 검색하여 찾아내고 넣었더니 통과했다...
