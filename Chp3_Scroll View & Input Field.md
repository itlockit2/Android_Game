# Chp3 UI

## Scroll View

1. Scroll View
		
	1. Scroll View 구성 요소
		*Scroll View Inspector
			* Scroll Rect (Script)	
			* Horizontal => 체크 시 수평방향으로 Scroll 가능
			* Vertical => 체크 시 수직방향으로 Scroll 가능
		* View Port
			* Content
			* Content로 사용자와의 Interaction 범위를 조절
			* Content의 Vertical(수직) Layout Group Component -> 내용물들 사이의 간격을 일정하게 조정하는 컴포넌트
			* 반대로, Content의 Horizontal(수평) Layout Group Component도 존재
			* View Port에는 Mask라는 Component가 있는데 이 Scroll View는 Mask가 가리키는 범위의 내용물만 보여줌
			* 따라서, View Port를 늘리면 Mask를 통해 볼 수 있는 영역이 늘어남
		* Scrollbar Horizontal
			* Sliding Area
		* Scrollbar Vertical
			* Sliding Area
	
<hr/ >

## Input Field

1. Input Field ?
	
	* 사용자가 데이터(캐릭터 이름, 패스워드 등)를 입력하는 창
	* Placeholder
		＊어떤 Text를 입력했을 때 자동으로 지워짐 (Enter Text... 부분)
	* Text
	* On Value Changed (String)
		* Input Text의 값이 변할 때 마다 Input Text에 대한 처리값을 출력함
	* On End Edit (String)
		* Button 필요없이 해당하는 Input Text를 입력한 뒤 Enter를 누르면 데이터에 대한 처리값이 출력 됨


