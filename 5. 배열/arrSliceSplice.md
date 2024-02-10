# 배열 자르기

```js
const arr = [0, 1, 2, 3, 4];

arr.splice(시작인덱스, 개수);

// 인덱스 1부터 2개를 제거한다.
arr.splice(1, 2); // arr:[0,3,4]

const result = arr.splice(1, 2);
console.log(result); // [1, 2]
```

---

```js
const arr = [0, 1, 2, 3, 4];

arr.slice(시작인덱스, 끝인덱스);

// 인덱스 1부터 3전까지 가져옴
arr.slice(1, 3);

const result = arr.slice(1, 3);

console.log(result); //[1, 2]
```
