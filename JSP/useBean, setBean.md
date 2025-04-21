## 사용법

```jsp
<jsp:useBean id="" class="" scope="" />
```

id: 페이지 내에서 사용할 변수 이름
class: 클래스가 위치한 경로
scope: page, request, session, application

## setProperty
```jsp
<jsp:setProperty name="" property="" />
```

name: useBean의 id값과 동일
property: \*(애스터리스크) 입력

## 예제
```jsp
<jsp:useBean id="people" class="a.b.People" scope="page"/>
```

a 패키지에 있는 b 패키지 밑의 People 클래스를 가지고 온다.

가지고온 People 클래스는 people라는 이름으로 접근 가능하다.

만약 문제에서 name과 age 속성을 다룬다는 내용이 있으면 getName, setName, getAge, setAge가 있다고 생각하면 된다.

useBean의 id에 들어갈 값은 코드를 보면 알 수 있다.

`login.checkUser()` 이 코드에서 login처럼 듣도보도 못한 변수가 사용되고 있으면 이 변수를 useBean에서 선언한 것이다.