# 문제

```
개발ㅏ 원두는 앞으로의 계획을 세우기 위해 분기별로 일정표를 짜려고 합ㄴ디ㅏ.

좀 더 편한 계획을 위해 원두는
해당 월을 입력하면 몇 분기인지 number 형태로 알려주는 알고리즘을 만들려 합니다.

특정월이 month(매개변수)로 주어질 때, month는 몇 분기에 해당하는지 return 하는 함수 solution을 완성하세요.
```

# 제한 사항

```
1. 1 <= month <=12
2. 소수점을 올림 하는 Math.ceil()을 사용해주세요.
```

---

`입출력 예시`

| month | return |
| :---: | :----: |
|   4   |   2    |
|  12   |   4    |

---

```js
function solution(month) {
  return Math.ceil(month / 3);
}

solution(4);
solution(12);
```
