while 반복문은 조건문이 true 일 경우
코드가 계속 반복되어 실행된다.

즉 true일 동안 해당 코드를 반복 실행한다.

```js
let age = 16;

while (age < 20) {
  console.log("현재나이", age);
  age = age + 1;
}

console.log("end");

// 현재나이 16
// 현재나이 17
// 현재나이 18
// 현재나이 19
// end
```

---

continue는 만나게 될 경우 명령문의 실행을 종료하고 다음 반복을 실행한다.

```js
let age = 16;

while (age < 20) {
  age = age + 1;
  if (age === 19) continue;
  console.log("현재나이", age);
}

console.log("end");

// 현재나이 17
// 현재나이 18

// 19 라는 값이 충족되었기에 continue가 실행되어 아래 console.log는 종료된다.
// 20 일때 명령문이 다시 실행되고 while문이 종료된다.

// end
```

---

break를 만나게 될 경우 while문이 종료가 된다.
또는 while 문 종료 후 실행시킬 다음 코드가 없다면 return을 사용해도 된다.

둘의 차이는 break는 while문만 종료하고 함수 전체의 코드 종료를 원하지 않을때 사용한다.

```js
let age = 16;

while (age < 20) {
  age = age + 1;
  if (age === 19) break;
  console.log("현재나이", age);
}

console.log("end");

// 현재나이 17
// 현재나이 18
// end
```
