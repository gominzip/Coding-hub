# 🔎 게임개발

https://www.acmicpc.net/problem/1516

## 💡 아이디어

- 위상정렬을 활용하여 각 건물의 최소시간을 업데이트한다.

## ✔ 문제풀이

- 위상정렬을 활용하되 빌딩 시간과 건설 완성 시간을 따로 담는다.
  - 위상을 돌 때마다 기존 next에 있는 건물 총 시간이랑 current + next 빌딩 시간을 비교해야하기 때문
- 그 이외에는 위상정렬을 활용한다.

## 🤕 어려웠던 점

- 위상정렬이 익숙하지 않았다... 다익스트라만 해야겠다 생각했는데 바로 이렇게 나올줄 몰랐...
  - python까지 복습을 하고나서 좀 익숙해진 느낌!
