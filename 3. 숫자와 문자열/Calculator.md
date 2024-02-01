# 문제

```
개발자 원두는 회사에서 덧셈 계산기를 만들어오라는 업무를 지시 받았습니다.
하지만 만들어간 덧셈 계산기는 제대로 작동하지 않았고

선배에게 피드백으로 '문자열은 숫자로 변환해야지!' 라는 말을 듣게 됩니다.
그래서 원두는 계산기에 입력된 값이 어떤 타입인지 확인하는 함수를 만들어보려 합니다.

입력값이 num1(매개변수)과 num2(매개변수)로 주어질 때 입력된 값이
각각 어떤 타입인지를 return하는 함수 solution을 만들어주세요.
```

# 제한 사항

```
1. num1, num2의 길이는 1이상 100이하 입니다.
2. num1, num2는 문자열 또는 숫자로 표기된 숫자입니다.

```

---

`입출력 예시`

| num1 | num2 |    return     |
| :--: | :--: | :-----------: |
| "9"  |  10  | string number |
|  19  |  1   | number number |
| "2"  | "14" | string string |

---

```js
function solution(num1, num2) {
  const num1Type = typeof num1;
  const num2Type = typeof num2;
  return `${num1Type} ${num2Type}`;
}

solution("9", 10);
solution(19, 1);
solution("2", "14");
```
