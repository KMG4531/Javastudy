자바는 이클립스라는 프로그램을 사용합니다.

[ECLIPSE](https://www.eclipse.org/downloads

여기서 다운받으시면 됩니다.


첫번째! 

```java
package basic;

public class Test01 {
	public static void main(String[] args) {
		// 나의 첫 자바프로그램
		System.out.println("ㅎㅇㅎㅇ");
		System.out.println("Hello,Java!");
		// 저장: ctrl + s
		// 실행: ctrl + F11
        // 단축키 ; sysout +(ctrl + 스페이스)
	}
}
```

결과

```java
ㅎㅇㅎㅇ
Hello,Java!
```

출력되어 나온다.

두번째!

```java
package basic;

public class Test02 {
	public static void main(String[] args) {

		// sysout: ()안의 문장을 console에 출력하는 명령어

		System.out.println("ABC");
		System.out.println(10 + 20);
		System.out.println("ABC+10");// 문자열 더하가 =붙여라="ABC10"
		System.out.println("3.14*10");
		System.out.println(10 + 20 + "ABC");
		System.out.println(10 + 20 + "ABC" + 10 + 20); // "ABC10"+20,두개씩 붙여라
		System.out.println(10 + 20 + "ABC" + (10 + 20));
	}
}
```

결과

```java
ABC
30
ABC+10
3.14*10
30ABC
30ABC1020
30ABC30
```

쭉 출력이 됩니다.
