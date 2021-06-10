이번 시간에는 Scanner를 조금 더 깊숙이 알아가보려고 합니다.

Scanner란?

키보드로 입력될 값을 프로그램으로 가져올 심부름꾼 역할의 객체

이 객체의 이름을 sc라고 정함 ( 이름 마음대로 정할 수 있음 )
 
메인 메소드에 1줄만 있으면 됨. (sc를 사용하기 전에 미리 만들어 둠)
 
정수 입력받을 때 : sc.nextInt()

실수 : sc.nextDouble()

문자열 : sc.next() 혹은 sc.nextLine()

한 단어만 한 줄 (띄어쓰기 포함 가능)
 
밑에 예시를 봅시다.
 
```java

package basic;
import java.util.Scanner;  // Scanner는 이 문장이 꼭 필요함! 

public class Test01 {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in); 

		String name;
		int age;
		double height;
		String address;
		
		System.out.print("이름:");
		name = sc.nextLine(); // 입력 받은 데이터를 1단어(String)으로 인식하여 name에 저장
		
		System.out.print("나이:");
		age = sc.nextInt(); // 입력 받은 데이터를 정수로 인식하여 age에 저장
		
		System.out.print("키:");
		height = sc.nextDouble(); // 입력받은 데이터를 실수(double)로 인식하여 height에 저장
		
		System.out.print("주소:");
		sc.nextLine(); // nextLine() 실행 전, 이전에 nextXXX()가 실행되었다면 이 한 줄을 추가해야 됨
					   // 엔터를 대신 먹어주는 역할
		address = sc.nextLine(); // 입력 받은 데이터를 String으로 인식하여 address에 저장
		
		System.out.println("==== 사용자 정보 ====");
		System.out.println("이름 : " + name);
		System.out.println("나이 : " + age + "세");
		System.out.println("키 : " + height + "cm");
		System.out.println("주소 : " + address);
		// 1개의 데이터를 인식하는 기준은 띄어쓰기 혹은 엔터
		
	    sc.close(); // 심부름꾼 삭제 (생략 가능) 
	}
}
```
[실행]

```java
이름:
나이:
키:
주소:
```

여기에 입력을 해주고 실행을 시키면
```java
==== 사용자 정보 ====
이름 : 주먹왕 랄프
나이 : 34세
키 : 204.0cm
주소 : 게임 속
```

이런식으로 코드가 나옵니다.
