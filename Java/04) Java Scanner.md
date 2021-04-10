
Scanner라는 것은 java.util 패키지에 포함된 클래스이다.

쉽게 말해서 사용자 값으로부터 정보들을 입력하면 받아들이는

함수라고 생각하면 됩니다.


'초'를 사용자에게 입력받고 이를 x 분 x 초를 계산해주는 것을 만들어 주겠습니다.

```java
package basic;

import java.util.Scanner;

public class Test01 {
	public static void main(String[] args) {
	   
        Scanner sc = new Scanner(System.in);

		System.out.println("초;");

		int sec = sc.nextInt();  // 정수 1개를 입력받고, 이를 sec에 저장
		System.out.println("입력 값;" + sec + "초");
		System.out.println(sec / 60 + "분" + sec % 60 + "초");
	}
}

```

출력

```java
초;
```
