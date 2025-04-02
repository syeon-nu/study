## Request 객체
Request 객체는 유저의 요청에 대한 다양한 정보를 가지고 있다. jsp에서 `request` 변수명을 통해 사용 가능하다.

`request.getParameter("키값")`으로 키값에 해당하는 밸류값을 가지고 올 수 있다.

예)
`naver.com/login?id=seoyeon&password=123`

`request.getParameter("id")` = `"seoyeon"`
`request.getParameter("password")` = `123`