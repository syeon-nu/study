## `input`

사용법: 
```html
<input type="" name="" value=""/>
```

* type: "text", "date", "password", "number"등 입력받고 싶은 데이터의 형식을 지정해주면 input 태그가 그에 맞게 바뀐다.
* name: 파라미터를 넘겨줄 때 name에 적힌 값으로 파라미터를 전달한다.
* value: input에 들어갈 값이다.

`<input name="이름" value="서연"/>`의 값을 `서연의홈페이지/main`으로 보내게 되면 `서연의홈페이지/main?이름=서연` 형식으로 전달된다.

그럼 jsp에서는 이를 `<%= request.getParameter("나이"); %>`을 통해 `"서연"`이라는 값을 가지고 올 수 있다.