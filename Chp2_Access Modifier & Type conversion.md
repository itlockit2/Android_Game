# Chp2 Access Modifier & Type conversion 

## Access Modifier

1. 접근 한정자
		
	* public // public 으로 선언된 변수는 Engine에서 수정 가능
	* private // 감춰져 있기 때문에 Engine에서 수정 불가
	* internal // 어셈블리 내부 
	* protected 
	* protected internal // 같은 어셈블리 내부 & 파생 클래스
	
	* 당연한 이야기지만, 자료형에 맞게 값을 입력해주어야 함

<hr/>

## Type conversion

1. 형 변환
		
		* 자료형을 변환하는 것 ( 게임화면에서 점수를 보여 줄 때 int나 float를 string으로 변환해야 함 )
		* 명시적 형변환
			* 사용자가 직접 형변환을 해주어야 하는 것
				float -> int
				string -> int 
				int -> string
				int.ToString("형식"); -> int 부분에 정수를 넣어줌
				string -> int
				int.Parse(string);
				float -> int
				(int)float
		* 암시적 형변환
			* 컴퓨터가 알아서 해주는 형변환
				int -> float
				string + int
				"점수 : " + 100
				"점수 : 100"

<hr/>
 
	