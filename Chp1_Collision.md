# Chp1 Collision

## Collision

1. Collsion 충돌

	1. 두 Object 모두 Collider(2D) 를 가지고 있다. 
		* Collider -> Object의 충돌 영역 
		* 2D 게임에서는 뒤에 2D가 붙은 Collider를 사용 
	2. 둘 중 적어도 하나는 Rigidbody(2D) 를 가지고 있다.
	Rigidbody -> 물리 엔진 Component (중력 작용)
		* Mass = 질량, 떨어졌을 때 충격량이 증가함
		* Linear Drag = 직선 저항, 물체가 직선 운동을 할 때 얼마나 저항을 줄 것인지에 대한 값
		* Angular Drag = 회전 저항, 물체가 회전 운동을 할 때 얼마나 저항을 줄 것인지에 대한 값 
		* Gravity Scale = 중력 가속도, 1이면 아래로 떨어짐 / -1이면 위로 올라감 / 0이면 무중력 상태 
		* Constraints = 물체의 특정 position을 고정시키고 싶을 때 사용 
	3. Rigidbody(2D) 를 가진 Object가 움직인다.

<hr/>

2. Trigger 충돌

	1. 두 Object 모두 Collider(2D) 를 가지고 있다. 
	2. 둘 중 적어도 하나는 Rigidbody(2D) 를 가지고 있다.
	3. 둘 중 적어도 하나는 IsTrigger 옵션이 체크되어 있다.
	4. Rigidbody(2D) 를 가진 Object가 움직인다.
		
