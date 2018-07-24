# Chp4 Animation

## Animation Controller

1. Animation Controller 
		
	* Base State - 기본적으로 존재하는 State
		1. Any State 
			* 상태전환 대기 
			* 우리가 만든 모든 State가 특정 조건을 만족했을 때 Transition이 향하는 State로 이동 
		2. Entry - 맨 처음 시작할 Animation State를 지정해주는 역할
		3. Exit 
			* Animation 종료 상태를 지정 
			* 다시 Entry로 돌아오기 위해 사용
		
	* Animator Inspector 
		* Speed - Clip을 재생하는 속도
	
	* State를 더블 클릭하면 하나의 Clip에 대한 3가지의 Inspector 요소 출력
		* Loop Time - Clip을 반복해서 재생할 것인가의 여부
		* Loop Pose - 처음과 끝의 격차가 너무 크면 반복 재생시 이질감이 있기 때문에 그 간격을 부드럽게 맞춰주는 역할
		* Cycle Offset - 반복을 시작할 위치
	
	* 어떤 조건에 따라 Transition을 변화시키고 싶다면 Animator의 Parameters 기능 이용
		* Trigger - 한 번 실행되면 자동으로 False가 되는 Trigger
		* 만든 Trigger와 같은 값들은 Transition Inspector의 Conditions 부분에 추가 함으로서 사용 가능
	
	* Transitions Inspector 
		* Has Exit Time 
			* Check 되어 있으면 이전 상태가 종료되어야만 전환이 가능
			* 반대로, 해제 되어 있으면 언제든지 조건만 만족하면 전환이 가능
		* Settings
			* Has Exit Time Check시 현재 State를 완벽히 끝내고 전환하고 싶으면 Exit Time은 1로 설정
			* Transition Duration - Animation을 전환할 때 얼마만큼 겹치면서 전환을 할 건지 설정하는 요소
			* Transition Offset - Animation을 전환할 때 얼마만큼 겹치면서 전환을 할 건지 설정하는 요소
				* 주로, 3D에서 많이 사용 
		
2. 파라미터 변경

	* C# Script를 통해 특정 조건을 만족 시 그 Animation을 수행하도록 만듬
	* SetInteger
	* SetFloat
	* SetBool
	* SetTrigger
	
	* GetComponent< Animator >().GetFloat("Hp_f"); 
	* GetComponent< Animator >().SetFloat("Hp_f", 100); 등등 

