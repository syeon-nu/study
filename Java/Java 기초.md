# Java 기초

## 코드 실행법
컴퓨터 입장에서는 코드를 어디서부터 실행해야 할지 모르기 때문에 main함수를 만들어야 한다(모든 언어 공통)
```java
class A {  
    public static void main(String[] args) {  
  
    }  
}
```

## 입력과 출력

### 입력
```java
Scanner scanner = new Scanner(System.in);  
String result = scanner.nextLine();  
System.out.println(result);
```

### 출력
출력은 `sout`를 입력하면 자동으로 `System.out.println()`을 만들어준다.


