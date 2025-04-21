## 사용법
param 액션 태그는 오로지 include 액션 태그, forward 액션 태그 사이에서만 사용된다.

## include 태그에 사용한 경우

```jsp
<!-- index.jsp -->
123
<jsp:include page="login.jsp">
	<jsp:param name="seoyeon" value="hello"/>
</jsp:include>
```

index 페이지에서 login 페이지를 포함한다. param 액션 태그를 통해 login 페이지에 seoyeon = "hello"를 전달한다.

```jsp
<!-- login.jsp -->
<p>여기는 로그인 페이지</p>
<%= request.getParameter("seoyeon") %>
```

결과:

```html
<!-- 주소는 index.jsp -->
123
<p>여기는 로그인 페이지</p>
hello
```

## forward 태그에 사용한 경우

```jsp
<!-- index.jsp -->
123
<jsp:forward page="login.jsp">
	<jsp:param name="seoyeon" value="hello"/>
</jsp:include>
```

index 페이지에서 login 페이지로 이동한다. 주소는 여전히 index.jsp이다. param 액션 태그를 통해 login 페이지에 seoyeon = "hello"를 전달한다.

```jsp
<!-- login.jsp -->
<p>여기는 로그인 페이지</p>
<%= request.getParameter("seoyeon") %>
```

```html
<!-- 주소는 index.jsp -->
<p>여기는 로그인 페이지</p>
hello
```

## \<%@ include %>와 <jsp:include/> 차이

```jsp
<%@ include file="login.jsp" %>
<jsp:include file="login.jsp" />
```

골뱅이가 붙은 include는 file(골아파)을 불러온다. file을 통째로 불러오기 때문에 실행 전 코드가 남아있어 코드에 있는 변수를 사용할 수 있다.

반대로 jsp:include는 (이미 작업이 끝난)page를 가지고 오기 때문에 코드가 실행된 결과값만이 나타난다.