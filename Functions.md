# Chp2 Functions

## Functions

1. 다양한 함수들 (정의되어 있는 함수들)
		
	* Debug.Log
	* Destroy
	* Translate
	* Rotate
	* GetKeyDown
	* Instantiate
	* GetComponent
	
	1. Debug.Log
		
		* Debug.Log("Hello World");
		* 괄호 안의 내용을 Console창에 표시 
	
	2. Destroy
		
		* Destroy(gameObject);
		* 괄호안의 Object를 없앰
		* Destroy(gameObject, 3f);
		* 괄호안의 Object를 몇초 뒤에 없앰, 3f는 3초 뒤를 의미, f는 float를 의미하므로 실수초도 지정 가능
	
	3. Translate	
		
		* transform.Translate(1f, 0f, 0f);
		* 게임오브젝트를 괄호 안의 좌표(x, y, z)만큼 이동시킴  
		* transform.Translate(Vector3.right);
		* Vector3는 x, y, z 모든 좌표를 가지고 있는 자료형
		 ![Vector3](images/Vector3.png)
		* 위의 Vector3 함수들을 사용하여 이동시키는 것도 가능하며 추천하는 방법 

	4. Rotate

		* transform.Rotate (0f, 0f, 1f);
		* 게임오브젝트를 괄호 안의 좌표(x, y, z)만큼 회전시킴
		* 또한, 괄호 안에 Vector3도 넣어 줄 수 있음
		* z 좌표의 양의 회전 값은 시계 반대 방향으로 돌아감

	5. GetKeyDown

		* Input.GetKeyDown(KeyCode.Space)
		* 특정 키가 눌리는 순간 true를 반환 
		* 위의 경우, Space가 눌리면 true를 반환

	6. Instantiate

		* Instantiate (gameObject);
		* 괄호 안에 있는 게임오브젝트를 복제 

	7. GetComponent

		* GetComponent<SpriteRenderer>().color = Color.red;
		*                      <컴포넌트 이름>()
		* 현재 게임 오브젝트의 다른 컴포넌트를 가져오는 함수
		* Transform이 아닌 다른 컴포넌트를 가져오기 위해선 꼭, GetComponent를 해야함

2. 이벤트 함수

	* 실행되는 시점이 미리 정해져 있는 함수들
	* Start / Update / OnCollisionXXX
	
	1. void OnCollisionEnter2D(Collision2D col){}
		* Collision 충돌 시 호출되는 함수
		* Parameter는 충돌한 상대방 물체 정보
	2. void OnCollisionStay2D(Collision2D col){}
		* Collision 충돌 중에 계속 호출되는 함수
	3. void OnCollisionExit2D(Collision2D col){}
		* Collision 충돌이 끝나는 순간 호출되는 함수
## Condition

1. 조건문

	* 조건문 (if-else문)
	* 논리 연산자 (==, >=, >, <=, <)
	* 산술 연산자 (+, -, *, /, %)	
	* Console View의 Collapse기능 
		* 결과값이 같은 것들을 합쳐서 최신 결과값만을 출력해 줌
		* 해제하면 합치지 않고 모두 표시
	
<hr/>

## Vector3

1. Vector3 ?

	* (x, y, z)로 이루어진 자료의 형태
	* x, y, z의 정점으로부터 크기와 방향을 나타내는 것

	1. 벡터의 연산 
		* 더하기와 빼기가 가능  
		* 벡터끼리의 곱셈은 불가능
		* 벡터에 상수를 곱하는 것은 가능 
		* 또한, 상수를 나누는 것도 가능
		* 상수를 곱하거나 나누는 것은 벡터의 방향은 유지를 하되 크기를 조절할 때 많이 사용

	2. 기본적인 Vector3 함수
		![Vector3](images/Vector3.png)

		* 정의되어 있지 않은 새로운 벡터를 만들 때에는 new Vector3 (x, y, z)를 통해 만들어 줌

<hr/>

2. Trigger 충돌

1. 두 Object 모두 Collider(2D) 를 가지고 있다. 
2. 둘 중 적어도 하나는 Rigidbody(2D) 를 가지고 있다.
3. 둘 중 적어도 하나는 IsTrigger 옵션이 체크되어 있다.
4. Rigidbody(2D) 를 가진 Object가 움직인다.
	1. Project View
		![Project View](C:\Users\KJM\Desktop\MarkDownImage/ProjectView.png)

	* 게임에 사용되는 Asset들을 관리하는 창 
	* 윈도우의 탐색기와 비슷한 역할 
	* 다양한 검색 기능
	* 폴더 생성 및 Image 파일 불러오기 

	2. 새로운 폴더 만들기
	
	* Asset 창에서 마우스 우클릭 후 Create를 통해서 만듬
	* Import를 시키는 경우는 파일을 Drag & Drop을 통해 간단히 넣어줄 수 있음 
	* Asset Search 
		![Project View](C:\Users\KJM\Desktop\MarkDownImage/AssetSearch.png)
	* 어떤 특정한 타입만을 보고 싶은 경우 검색창 오른쪽 버튼( Search By Type )을 통해 특정한 Type만 검색 가능 
<hr/>
 
	2. Hierarchy View