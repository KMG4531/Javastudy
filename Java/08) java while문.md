## < while문 >

형식 :

while( 조건식 ) {

 // 조건식이 true면 실행할 문장

}

### 실행 순서

조건식 검사 --> true면 --> { } 실행 -->

조건식 검사 --> true면 --> { } 실행 --> 

... --> false면 --> while문 종료

### [while문을 이용한 소스코드]

```java
package basic;
public class Test01 {
	public static void main(String[] args) {
		// 1 ~ 10 출력
		int num = 1;
		while(num <= 10) {
			System.out.println(num);
			++num; // num++; 해도 됨
		}
		System.out.println("마지막 num의 값 : " + num);
	}
}
```

실행을 시켜주시면

```java
1
2
3
4
5
6
7
8
9
10
마지막 num의 값 : 11
```
