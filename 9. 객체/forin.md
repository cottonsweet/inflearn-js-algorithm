# 문제

```
원두는 사내 볼링 대회의 등수별 수상자의 상품을 정리하고 있습니다.
등수별 수상자의 인원이 적힌 객체 winners가 주어질 때,

해당 등수를 수상할 인원의 수에 맞게
배열에 담아 return하는 함수 solution을 완성해주세요.

예를 들어, 1위가 2명, 2위가 1명이라면 [1, 1, 2] 형태로 return 해주세요.
```

# 제한 사항

```
1. 객체 winners의 key는 1위부터 순서대로 주어집니다.
2. 객체 winners 각 속성의 key는 순위를 의미하여 1 이상 5 이하의 정수입니다.
3. 객체 winners 각 속성의 value는 인원을 의미하며 1 이상 5 이하의 정수입니다.
```

---

`입출력 예시`

|     winners     |        return         |
| :-------------: | :-------------------: |
| {1:1, 2:2, 3:4} | [1, 2, 2, 3, 3, 3, 3] |

---

```js
function solution(winners) {
  let result = [];
  for (const win in winners) {
    for (let i = 0; i < winners[win]; i++) {
      result.push(Number(win));
    }
  }
  return result;
}

solution({
  1: 1,
  2: 2,
  3: 4,
  // 4: 1,
  // 5: 2,
}); // [1, 2, 2, 3, 3, 3, 3]
```
