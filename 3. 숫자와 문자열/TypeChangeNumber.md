# 문제

```
똑똑한 개발자 원두는 피드백을 반영하여 덧셈 계산기를 개선하려 합니다.
문자열 타입으로 된 숫자를 입력해도 제대로 작동하도록 고쳐가기로 합니다.

입력값이 num1, num2로 주어질 때
입력된 값의 합을 return하는 함수 solution을 만들어주세요.
```

# 제한 사항

```
1. num1, num2의 길이는 1이상 100이하 입니다.
2. num1, num2는 문자열 또는 숫자로 표기된 숫자입니다.

```

---

`입출력 예시`

| num1 | num2 | return |
| :--: | :--: | :----: |
| "1"  |  2   |   3    |
|  5   |  6   |   11   |
| "3"  | "5"  |   8    |

---

```js
function solution(num1, num2) {
  return Number(num1) + Number(num2);
}

solution("1", 2);
solution(5, 6);
solution("3", "5");
```
