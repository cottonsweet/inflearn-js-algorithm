# 문제

```
개발자 원두는 피규어를 모은은 취미가 있습니다.
프로젝트에 성공하여 상여금을 받은 원두는
이 금액을 온전히 피규어 구매에 사용하고 싶습니다.

원두가 모으는 피규어의 가격은 개당 57,000원 입니다.
원두가 받게 되는 상여금 money원이 매개변수로 주어질 때
원두가 최대로 살 수 있는 피규어의 개수를 return 하는 solution 함수를 완성해 주세요
```

# 제한 사항

```
1. money는 0원 이상 100만원 이하의 number 입니다.
```

---

`입출력 예시`

| money  | return |
| :----: | :----: |
| 230000 |   4    |
| 769000 |   13   |
| 35000  |   0    |

---

```js
function solution(money) {
  return Math.floor(money / 57000);
}

solution(230000); // 4
solution(769000); // 13
solution(35000); // 0
```
