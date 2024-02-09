# 문제

```
개발자 원두는 담당하고 있는 프로젝트의 명세서를 작성하고 있습니다.
프로젝트에서 사용된 기술 스택의 이름이 배열 stacks로 주어질 때
내림차순으로 정렬하여 return하는 함수 solution을 완성해주세요
```

# 제한 사항

```
1. 배열 stacks의 길이는 1이상 10이하 입니다.
2. 배열 stacks의 각 단어의 길이는 1이상 10이하인 문자열 입니다.
3. 배열 stacks의 단어들은 영문 소문자로만 이루어져 있습니다.

```

---

`입출력 예시`

|                   stacks                   |                  return                   |
| :----------------------------------------: | :---------------------------------------: |
| ["typescript", "express", "node", "react"] | ["typescript", "react", "node", "express] |
|    ["docker", "graphql", "javascript"]     |   ["javascript", "graphql", "docker" ]    |

---

```js
function solution(stacks) {
  return stacks.sort().reverse();
}

solution(["typescript", "express", "node", "react"]);
solution(["docker", "graphql", "javascript"]);
```
