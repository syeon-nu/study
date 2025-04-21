```jsp
<!-- index.jsp -->
<html>
	<body>
		여기는 인덱스 페이지
		<jsp:forward page="login.jsp">
	</body>
</html>
```

```jsp
<!-- login.jsp -->
<html>
	<body>
		여기는 로그인 페이지
	</body>
</html>
```

실행 결과

```jsp
<!-- 그러나 주소는 index.jsp -->
<html>
	<body>
		여기는 로그인 페이지
	</body>
</html>
```

즉, forward 액션 태그는 해당 페이지로 이동하지만 주소는 현재 보여지고 있는 페이지(index.jsp)가 된다.