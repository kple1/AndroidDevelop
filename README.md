setContentView
자바 코드로 작성한 레이아웃 혹은 레이아웃 파일(XML)을 넘기면 해당 레이아웃이 화면에 표시된다.


new LinearLayout()
linearlayout 레이아웃을 만들 수 있다. this키워드가 들어가는데, 이는 Context객체를 의미한다. 일반적인 Context는 프로그래밍 언어에서 객체의 정보를 담고있는 것을 의미한다. 안드로이드에서 Context는 UI 구성 요소인 뷰에 대한 정보를 확인할 수 있도록 하는 객체이다.


setOrientation()
LinearLayout은 기본적으로 Vertical(세로방향), Horizontal(가로방향)을 지정해 주어야 한다.상수 LinearLayout.VERTICAL 혹은 LinearLayout.HORIZONTAL 중 하나를 넣어서 지정할 수 있다.


this 키워드
this키워드는 Context객체가 전달된 것이다. 안드로이드에서 new연산자를 사용해 뷰객체를 만들때는 항상 Context객체가 전달되어야 한다. LoadActivity에서  상속받은 AppConpatActivity클래스는 Context를 상속하므로, 이 클래스 안에서는 this를 Context객체를 사용할 수 있는 것이다. 만약 Context를 상속받지 않는 클래스라면, getApplicationContext라는 메소드를 호출해 앱에서 참조가 가능한 Context객체를 사용해야한다. 안드로이드에서 컨텍스트란 뷰에대한 정보를 가지고 있는 객체를 의미한다.


LayoutParams 객체
LayoutParam객체는 뷰 배치를 위한 속성을 설정할 수 있게해주는 객체이다. 이 객체는 레이아웃에 추가되는 뷰의 속성 중 레이아웃과 관련된 속성을 담고 있다. 가로와 세로는 필수 값이며, LayoutpParams의 상수 MATCH_PARENT, WRAP_CONTENT중 하나를 사용할 수 있다.


addView()
addView메소드를 사용하면, 레이아웃에 뷰를 추가할 수 있다. 

 
stetLayoutParams()
뷰 객체의 레이아웃 설정을 해준다
