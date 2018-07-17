# Chp1 Interface

## Interface

Create Project

	1. New 클릭
	2. Project Name 및 Template( 3D or 2D 설정 ) 설정
	3. Create Project 

기초적인 View 

	 Project View
	 Hierarchy View
	 Inspector View
	 Scene View 
	 Game View 

1. Project View
		![Project View](C:\Users\KJM\Desktop\MarkDownImage/ProjectView.png)

		 게임에 사용되는 Asset들을 관리하는 창 
		 윈도우의 탐색기와 비슷한 역할 
		 다양한 검색 기능
		 폴더 생성 및 Image 파일 불러오기 

* 새로운 폴더 만들기
	
		Asset 창에서 마우스 우클릭 후 Create를 통해서 만듬
		Import를 시키는 경우는 파일을 Drag & Drop을 통해 간단히 넣어줄 수 있음 
* Asset Search 
		![Search View](C:\Users\KJM\Desktop\MarkDownImage/AssetSearch.png)
		
			
		어떤 특정한 타입만을 보고 싶은 경우 검색창 오른쪽 버튼( Search By Type )을 통해 특정한 Type만 검색 가능 

2. Hierarchy View
		![Hierarchy View](C:\Users\KJM\Desktop\MarkDownImage/HierarchyView.png)
		
		 현재 Scene에 사용되는 GameObject를 관리하는 View
		 새로운 GameObject를 생성 / 삭제
		 계층 구조 설정 
	 	 마찬가지로 Hierarchy View에서 오른쪽 버튼을 통해 Object 생성이 가능
		 
* Main Camera

		User에게 어떻게 게임을 보여줄 지 보여주는 Camera
		Z축 잘 볼 것 
* 계층 구조화

		부모 자식 설정 즉, 그룹화와 유사 
		한 Object가 움직이면 같이 움직임
		자식 Object를 부모 Object에 넣으면 자식으로 들어가게 됨
		이 경우, 부모 Object를 움직이면 같이 움직이게 됨
 		Transform 속성을 그대로 따라가게 됨 
		
3. Inspector View
		![Inspector View](C:\Users\KJM\Desktop\MarkDownImage/InspectorView.png)
		
		현재 선택한 GameObject 또는 Asset의 정보를 보여주는 부분 
		Component 추가 / 삭제 / 변경
		GameObject 이름 / 태그 / 레이어 변경
			
* Transform Inspector

		위치 / 회전 / 크기를 정하는 Inspector
		모든 GameObject가 가지고 있음

* Sprite Renderer Inspector

		Flip 상하좌우 반전
		X -> 좌 / 우 Y -> 상 / 하 반전
		
* Sorting Layer / Order in Layer Inspector

		이미지의 출력 순서 	
		파워포인트의 그림 맨 뒤로 보내기 맨 앞으로 보내기와 유사 
		번호 순서로 Layer를 지정했다 하였을 때 1번 Layer가 가장 아래로 가며 큰 번호일 수록 가장 나중에 그려짐 (맨 위에 있음) 
		같은 Type의 GameObejct인 경우 Sorting Layer가 아닌 Order in Layer를 통해 조절 
		
		
		
		
		
		
		
		
		
		
		
		
		
		
