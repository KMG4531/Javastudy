
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

라고 뜹니다 여기에다 193초를 입력해 주겠습니다.
 
 ```java
초;
193
입력 값;193초
3분13초
```


이런 식으로 X 분과 X 초가 나옵니다.


이번에는 나이를 입력받고 중학생인지 아닌지를 판별해 주는 것을 만들어보겠습니다.

```java
package basic;

import java.util.Scanner;

public class Test02 {
	public static void main(String[] args) {

		Scanner sc = new Scanner(System.in);

		int age;

		System.out.println("나이를 입력하세요");
		age = sc.nextInt(); // 정수 1개 입력 받고, 이를 age에 저장

		System.out.println("당신의 나이;" + age);
		System.out.println("중학생?;" + (14 <= age && age <= 16));
	}
}

```
