## < 형 변환(casting) >

- 데이터의 자료형을 일시적으로 변경

### 1. 자동형 변환 : 컴퓨터의 판단하에 자동으로 해주는 형 변환

예) double num1 = 3; // 3 -> 3.0으로 자동형 변환되어 3.0 num1에 저장

sysout( 'A' + 1 ); // 'A'-> 65로 자동형 변환되어 66이 출력

10 / 3.0 // 10 -> 10.0로 자동형 변환되어 10.0 / 3.0으로 계산

### 2. 강제형 변환 : 개발자가 '형 변환 연산자'를 사용하여 강제로 하는 형 변환

sysout( (char)65 ); // 65 -> 'A'로 강제 형 변환

int num2 = (int)3.99999; // 3.99999 -> 3으로 강제 형 변환


< 자동형 변환해주는 기준 >

문자를 숫자로

정수를 실수로

작은 사이즈를 큰 사이즈로

==> 데이터 손실 우려가 없을 때 해줌

실제로 해봅시다.
```java

package basic;

public class Test01 {
	public static void main(String[] args) {

		double num1 = 3; 
		// int num2 = 3.0;  // 자동형변환 안해줌
		int num2 = (int)3.0; 
		
		char ch = 'A'; 
		ch = (char)(ch + 32); // (char) 없으면 에러남
		
		System.out.println(ch);
		
		System.out.println( (int) 3.99999999999 );
		
	}
}

```
