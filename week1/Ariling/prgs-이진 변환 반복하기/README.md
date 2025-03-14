# 🔎 이진 변환 반복하기

https://school.programmers.co.kr/learn/courses/30/lessons/70129

## 💡 아이디어

- "1"일 때까지 0을 제거하고 길이수를 이진수로 변환하고 다시 문자열로 변환하는 반복을 거치면 해결가능하다.

## ✔ 문제풀이

> **python && js**

- "1"일 때까지 다음과 같은 반복을 돌리면 된다.
  - for문을 돌려 0의 개수를 카운트하여 그 수 만큼 더하고 replace를 한다.
    - 여기서 js는 그냥 replace를 하면 하나만 바꿔주므로 replaceAll을 해야 한다.
  - 길이를 format메서드를 활용하여 이진수로 변환한 뒤 다시 문자열로 변환한다.
  - 위의 과정들이 끝나면 회차를 더한다.

## 🤕 어려웠던 점

- python의 경우 이진수로 바꾸는 bin()이라는 메서드가 있지만 할 경우 접두사가 붙어서 제대로 할 수가 없었다. 그래서 다른 메서드인 format을 검색해서 활용했다.
- js의 경우에는 toString(2)로 이진수를 만들 수 있다는 것을 검색을 통해 알아냈다.
