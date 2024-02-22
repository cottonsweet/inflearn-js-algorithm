# map 메서드

```js
const week = ["월", "화", "수", "목", "금"];

const result = week.map((요일) => "^_^" + 요일);

console.log(result); //  ["^_^월", "^_^화", "^_^수", "^_^목", "^_^금"];
```

---

# filter 메서드

```js
const numList = [1, 2, 3, 4, 5];

numList.filter((num) => num % 2 === 0);

// 결과: [2, 4]
// 원본배열인 numList: [1, 2, 3, 4, 5] (원본 배열은 수정되지 않음)
```
