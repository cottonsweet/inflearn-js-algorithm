# 문제

```
개발자 원두는 주말에 새로 식당을 창업한 친구를 도와주기로 했습니다.
식당은 개업 전 부터 인기가 많아 대부분의 예약이 완료된 상태.

식당은 장소가 매우 협소함으로 인해
앞으로 신청되는 예약은 여분의 자리가 있는지에 따라
예약이 가능 또는 불가 하다.

현재까지 예약된 손님 리스트 list, 수용 가능한 예약자 수 limit,
새로 예약 신청된 손님의 수 reports가 매개변수로 주어질 때,
현재까지 예약된 손님의 수 와 수용 가능한 손님의 수를 고려해
새로 예약을 신청한 손님을 받을 수 있는지를 boolean 타입으로
return 하는 함수 solution을 완성하세요.
```

# 제한 사항

```
1. list는 길이 1이상 10이하인 배열 입니다.
2. list의 원소는 1 이상 5이하인 정수 입니다.
3. limit는 1이상 15 이하인 정수 입니다.
4. reports는 1 이상 5이하인 정수 입니다.
5. while을 이용해서 문제를 풀어야 합니다.
```

---

`입출력 예시`

|     list     | limit | reports | return |
| :----------: | :---: | :-----: | :----: |
| [1, 5, 4, 3] |  15   |    3    | false  |
| [1, 1, 1, 2] |   7   |    2    |  true  |

---

```js
function solution(list, limit, reports) {
  let people = 0;
  let index = 0;

  while (index < list.length) {
    people = people + list[index];
    index = index + 1;
  }
}

solution([1, 5, 4, 3], 15, 3); // false
solution([1, 1, 1, 2], 7, 2); // true
```
