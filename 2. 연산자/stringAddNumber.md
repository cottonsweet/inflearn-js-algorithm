# 문제

```
개발자 원두는 사내 프로그램 테스트를 위한
테스트용 아이디를 만드는 업무를 받았습니다.

원두는 개발팀 팀원의 영어 이름과 생년월일 6자리를 뒤에 붙인 형태로
아이디를 만들기로 하였습니다.

개발팀 팀원의 영어 이름이 name(매개변수)으로 주어지고 생년월일이 birth(매개변수)로 주어질 경우
만들어지는 아이디를 return하는 함수 solution을 완성하세요
```

# 제한 사항

```
1. name은 string타입으로 제공됩니다.
2. birth는 number타입으로 제공됩니다.
3. name의 길이는 20을 넘지 않습니다.
4. birth는 항상 6자리 숫자로 제공됩니다.

```

---

`입출력 예시`

| name  | birth  |   return    |
| :---: | :----: | :---------: |
| marco | 971204 | marco971204 |
| tomas | 991108 | tomas991108 |

---

```js
function solution(name, birth) {
  return name + birth;
}

solution("marco", 971204);
solution("tomas", 991108);
```
