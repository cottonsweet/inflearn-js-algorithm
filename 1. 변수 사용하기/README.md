# let과 const

```js
const varibale = value;
let variable = value;
```

```
const 키워드는 선언과 동시에 값을 할당해야하며

let 키워드는 선언 이후의 초기값을 할당하지 않아도 선언이 가능하다.
```

```js
let age; // true
age = 20; // true



const age; // false
const age = 20 // true
age = 20 // false
```

```
const 키워드로 선언된 변수는 재할당이 불가하다.

let 키워드로 선언된 변수는 재할당이 가능하다.
```
