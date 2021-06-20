자바의 형태를 소개할꺼다.

원시자료형

데이터의 형태를 표기하는 8가지 자료형

## 1.정수형; 수숫점이 없는 숫자
 
* byte형 (1byte)

* short형(2byte) 

* int형(4byte); 정수데이터(정수 상수)의 기본자료형 

* long형(8byte)


## 2.실수형

* float형(4byte)

* double형(8byte) ; 실수데이터( 실수 상수)의 기본자료형


## 3.문자형

* char형(2byte) ; 문자상수의 기본자료형

* ; 문자상수) ''로 표현하는 1글자짜리 데이터

* 문자열상수) ""로 혀현하는 여러글자짜리 데이터


ASCII CODE ; 알파벳52개 , '0'~'9',특수기호66개 (총128문자)

UNICODE; 동양권 문자

'A'; 65

대문자 + 32 = 소문자


## 4.논리형(부울형)

* boolean(1byte)

* true, false 상수를 가지고 있다


## 5.문자열형

String형

원시자료형은 아니지만 원시자려형 취급이 가능함

문자열("")데이터의 기본자료형


[코드]
```java
package basic;

public class Test02 {
	public static void main(String[] args) {

		System.out.println(10000000000L);// L ; long형으로 처리한다

		System.out.println((char) 65);// A
		System.out.println((int) 'B');// 66
		System.out.println((int) '가');// 44032

		System.out.println(10 >= 20); // false

		System.out.println(1); // 전체에 + 0을 하면된다
		System.out.println(1.0); // 소수
		System.out.println('1'); // 아스키코드값
		System.out.println("1"); // 문자열값
		// 모두 같은 1일까?
	}
}
```

출력
```java
10000000000
A
66
44032
false
1
1.0
1
1
```
이런식으로 출력이 됩니다.
