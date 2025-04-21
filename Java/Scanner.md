# Scanner
입력을 위해 사용하는 클래스

```java
import java.util.Scanner;

public class IntroduceScanner {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		String a = sc.nextLine();
	}

}
```

## 메서드
### next()
다음 공백을 만나지 전 까지의 값을 **String**으로 저장
```java
import java.util.Scanner;

public class IntroduceScanner {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		
		String a = sc.next();
		String b = sc.next();
		String c = sc.next();
		System.out.println(a);
		System.out.println(b);
		System.out.println(c);
	}

}
```

### nextInt()
```java
import java.util.Scanner;

public class IntroduceScanner {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		
		int a = sc.nextInt();
		int b = sc.nextInt();
		int c = sc.nextInt();
		System.out.println(a);
		System.out.println(b);
		System.out.println(c);
	}

}
```
### nextLine()
엔터 누르기 전 까지의 값을 **String**으로 저장
```java
import java.util.Scanner;

public class IntroduceScanner {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		
		String a = sc.nextLine();
		String b = sc.nextLine();
		String c = sc.nextLine();
		System.out.println(a);
		System.out.println(b);
		System.out.println(c);
	}
}
```