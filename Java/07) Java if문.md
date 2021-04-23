## < if 문 >

형식 :

if( 조건식 ) {

조건식이 true 면 실행할 문장 ==> false 면 건너뜀

= if의 종속 문장

}

참고) 종속 문장이 1개라면 (...;) {} 생략 가능 (비추천)

if 문은 조건이 true 일 때만 실행되고, true가 아니라 false 면

else if로 넘어간다. else if 도 아니라면 else로 실행이 됩니다.

밑에 프로그램을 봅시다.

밑에 프로그램에서도 저번에 배웠던 Scanner를 쓸 겁니다.

Scanner를 모르신다면 Scanner 04, 05를 참고하세요.


```java
package basic;

import java.util.Scanner;

public class Test01 {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in); 
		int age;
		System.out.print("나이:");
		age = sc.nextInt();
		
		if (age >= 20) {
			System.out.println("성인입니다.");
		} 
		else { // 그렇지 않으면.. (위에 if가 짝꿍)
			// 위의 조건식이 false면 무조건 이걸 실행해
			System.out.println("미성년자입니다.");
		}
		
		if (age <= 7) {
			System.out.println("미취학 아동");
		} 
		else if(age <= 13) {
			System.out.println("초등학생");
		}
		else if(age <= 16) {
			System.out.println("중학생");
		}
		else if(age <= 19) {
			System.out.println("고등학생");
		} 
		else {
			System.out.println("대학생 혹은 일반 성인");
		}
	}
}
```

위에 보시면 성인과 미성년자를 구분할 수 있는 if와 else가 있습니다. if와 else 밖에 없는 이유는 구분해 줄게 2개뿐이니까 if와 else밖에 없겠죠.

그 밑에 있는 명령문은 if, else if, else가 쓰입니다.

나이별로 구분해 주기 위해서 if, else if, else가 쓰입니다.

실행을 시켜주면

```java
나이:
```

나이를 입력시켜주라고 뜹니다.

여기에 20살과 19살을 따로 입력해주겠습니다.

####  <성인>
  
```java
나이:20
성인입니다.
대학생 혹은 일반 성인

```

#### <미성년자>
```java
나이:19
미성년자입니다.
고등학생

```
