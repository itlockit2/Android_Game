# Chp5 Others

## Save And Load & Scene Management

1. Save & Load
		
	* Unity Save System
		1. Player Prefs 
			* 유니티에서 제공하는 단순한 저장 방식 
			* 키(Key)와 값(Value)으로 이루어져 있다
				* 키(Key) - 저장된 데이터의 고유 값 / 문자열 (String) 형식
				* 값(Value) - 저장된 데이터 / 정수,실수,문자열 형식
			* 큰 용량의 데이터는 다루기 힘듬

		2. 데이터 저장하기
			* PlayerPrefs.SetInt(Key, Value) -> 정수형 데이터 저장
			* PlayerPrefs.SetFloat(Key, Value) -> 실수형 데이터 저장
			* PlayerPrefs.SetString(Key, Value) -> 문자열 데이터 저장
			* Key에 해당 Data를 저장한다

		3. 데이터 불러오기
			* PlayerPrefs.GetInt(Key) -> 정수형 데이터 로드
			* PlayerPrefs.GetFloat(Key) -> 실수형 데이터 로드
			* PlayerPrefs.GetString(Key) -> 문자열 데이터 로드
			* 즉, Key에 저장된 값을 불러온다
			* 만약, Key값에 지정된 값이 없으면 정수나 실수는 0을 리턴 
			* String은 빈 문자열 리턴 
			* 또한, 지정된 값이 없으면 Get함수에 Parameter로 default 값(기본 값)을 지정하여 그 값을 리턴되게 할 수 있음

2. Scene Management	

	1. Scene
		* Game Object가 배치되어 있는 파일
		* 메인 메뉴, 레벨 등을 하나의 Scene으로 만듬 
		
		* Scene 셋팅 하기
			1. File -> Build Settings 선택 (Ctrl + Shift + B)
			2. 그 후, Scenes In Build에 게임에 사용할 Scenes를 넣어줌
				* Scenes In Build의 왼쪽 -> 사용하는 Scene의 경로와 이름이 나옴
				* Scenes In Build의 오른쪽 -> 해당 Scene의 번호
					* 0번 Scene은 App을 켰을 때 가장 먼저 실행될 Scene을 의미
	
		* Scene 전환하기
			* Scene 전환을 위해서 Script 최상단에 Using UnityEngine.SceneManagement;를 사용하여야 함 
			* SceneManager.LoadScene(Scene 번호) -> 해당 번호의 Scene을 Load
			* SceneManager.LoadScene(Scene 이름) -> 해당 이름의 Scene을 Load
 


