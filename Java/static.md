```java
class A {
	static String sharedText = "기본";
}

class B {
	public static void main(String[] args) {
		A.sharedText = "바꾼값"; // A에 .을 찍어서 static에 접근
	}
}
```

static 변수는 class에서 공통적으로 사용되는 값이다.

```java
class A {
	int a = 1;
}

class B {
	public static void main(String[] args) {
		A a1 = new A();
		A a2 = new A();

		// a1은 5, a2는 10의 값을 가진다.
		a1.a = 5;
		a2.a = 10;
	]
}
```

```java
class A {
	static int a = 1;
}

class B {
	public static void main(String[] args) {
		A.a = 10; // a1, a2가 아니라 클래스 그 자체에서 접근한다.
	]
}
```