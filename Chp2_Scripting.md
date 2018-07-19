# Chp2 Scripting

## Scripting

1. Scripting을 하는 이유 ?

	* 우리가 원하는 Component를 만들기 위해서 
	* Unity가 지원해 주는 것 만으로는 한계가 있음

1. 기본 구조
	1. Script 생성 방법
		1. Asset창에서 마우스 오른쪽 클릭
		2. Create 
		3. C# Script 클릭

	2. Script 기본 구성
			
			// 아래 내가 작성할 Script에 이러한 기능들을 사용하겠다. 
			using System.Collections;
			using System.Collections.Generic;
			using UnityEngine;
		
			// Script의 이름(Test) 
			// MonoBehaviour가 있어야 Script를 Component로 사용할 수 있음
			public class Test : MonoBehaviour {

			// Use this for initialization
			// 이 Component가 맨 처음 시작될 때 '한번' 실행되는 함수
			void Start () {
		
			}
	
			// Update is called once per frame
			// 매 frame마다 한번씩 실행되는 함수
			void Update () {
		
			}
				}
	

2. 변수와 자료형
	
		기본적으로 C++의 자료형(int, float, string ....)과 같음
		Debug.Log("Hello World");
			-> Console view에 메세지를 보내고 싶을 때 사용하는 함수
		Console view의 Clear on Play 시능
			-> Play할 때 마다 Debug.Log를 비우고 실행한 Play 결과를 출력

3. 변수의 사용 범위

		void Start() 내부에 선언한 변수들은 지역 변수
		
		따로 선언하지 않아도 사용가능한 변수들
			* gameObject (game 부분 소문자 주의)
				현재 스크립트가 사용되고 있는 게임 오브젝트를 지칭하는 변수
			* transform (소문자 주의)
				현재 스크립트가 사용되고 있는 게임 오브젝트의 Transform 컴포넌트를 지칭하는 변수 
