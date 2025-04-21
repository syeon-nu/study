## include 디렉티브 태그

```jsp
<!-- include 디렉티브 태그 -->
<%@ include file = "login.jsp" %>
```

include 디렉티브 태그는 jsp가 실행되기 전 코드 "그 자체"를 가지고 온다.
## include 액션 태그

```jsp
<!-- include 액션 태그 -->
<jsp:include page="login.jsp"/>
<!-- 또는 -->
<jsp:include page="login.jsp"></jsp:include>
```

include 액션 태그는 jsp가 실행된 후 결과물(html)을 가지고 온다.

여기서 실행 전후가 무슨 뜻일까?

```jsp
<html>
	<body>
		<%! String a = "hi";%>
		<%= a %>
	</body>
</html>
```

위 코드의 실행 결과

```jsp
<html>
	<body>
		hi
	</body>
</html>
```

즉 include 디렉티브 태그는
```jsp
<body>
	<%! String a = "hi";%>
	<%= a %>
</body>
```

이 코드 자체를 가지고 오는 거라 a라는 변수를 사용 가능하고, include 액션 태그는 실행 결과

```jsp
<body>
	hi
</body>
```

위 코드를 가지고 오는거라 a 변수에 접근할 수 없다.