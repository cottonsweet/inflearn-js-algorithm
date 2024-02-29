# 문제

```
개발자 원두는 사용자가 검색창에 검색어를 한 글자씩 작성하면
해당 검색어를 포함한 추천 검색어를 추천해주는 프로그램을 만들려고 합니다.
여러 가지 데이터들을 모아 추천해주고 싶은 검색어 목록은 배열로 이미 완성하였습니다.
하지만 추천 목록을 언제까지 노출해야 할지 고민입니다.

사용자가 작성하려고 하는 검색어를 의미하는 문자열 search와
추천해줄 검색어 목록을 의미하는 배열 recommends가 주어질 때
검색어 목록에 전부 해당하는 가장 긴 문자열을 return하는 함수 solution을 완성하세요.
```

# 제한 사항

```
1. search는 길이 1 이상 200 이하인 문자열 입니다.
2. 배열 recommends의 길이는 3 이상 100 이하입니다.
3. 배열 recommends의 각 요소의 길이는 1 이상 200 이하인 문자열입니다.
4. search와 배열 recommends의 단어들은 영어 소문자로만 구성되어 있습니다.
```

---

`입출력 예시`

|  search   |          recommends          | return |
| :-------: | :--------------------------: | :----: |
| "flutter" | ["flower", "flow", "flight"] |  "fl"  |
|  "apple"  |  ["dad", "racecar", "car"]   |   ""   |

---

```js
function solution(search, recommends) {
  for (let i = search.length; i > 0; i--) {
    const searchKeyword = search.slice(0, i);
    for (let j = 0; j < recommends.length; j++) {
      const keyword = recommends[j];

      if (keyword.startsWith(searchKeyword) === false) {
        break;
      }
      if (j === recommends.length - 1) {
        return searchKeyword;
      }
    }
  }
  return "";
}

solution("flutter", ["flower", "flow", "flight"]); // "fl"
solution("apple", ["dad", "racecar", "car"]); // ""
```
