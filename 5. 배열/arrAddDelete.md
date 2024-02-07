# 배열에 요소 추가/제거하기

```js
// 배열에 요소 추가
const arr = [1, 2, 3, 4];

arr.push(5);
// push 메서드는 배열 요소의 맨 뒤에 추가한다.

console.log(arr); // [1, 2, 3, 4, 5]
```

---

```js
// 배열에 요소 제거
const arr = [1, 2, 3, 4];

arr.pop();
// pop 메서드는 배열 요소의 맨 뒤를 제거한다. (특정 요소 지정은 불가하다)

console.log(arr); // [1, 2, 3]

const removeValue = arr.pop();
// 해당 변수에는 배열에 제거된 요소 값이 할당된다.

console.log(removeValue); // 3
```

---

```js
// 배열 맨 앞의 요소 추가
const arr = [1, 2, 3, 4];

arr.unshift(5);
// unshift 메서드는 요소를 배열의 맨 앞에 추가한다.

console.log(arr); // [5, 1, 2, 3, 4]
```

---

```js
// 배열 맨 앞 요소 제거
const arr = [1, 2, 3, 4];

arr.shift();
// shift 메서드는 배열의 맨 앞 요소를 제거한다.

console.log(arr); // [2, 3, 4]

const removeValue = arr.shift();
// 해당 변수에는 제거된 요소 값이 할당된다.

console.log(removeValue); // 1
```
