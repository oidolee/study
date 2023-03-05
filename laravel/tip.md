   
   
   @if( !auth()->user() ){
        <h1 class="text-3xl text-center mt-20">Hello world!</h1>
    }@endif
    
    
    위 아래 쌍 써줘야함
    
    **
    no 필드로 auto_increment로 만들거 id 필드를 만들었다 이것을 찍으니
    ![image](https://user-images.githubusercontent.com/85022962/222957279-283b3f09-798d-40e5-ac36-f1eb844b1f1a.png)
      위 처럼나와 아래처럼 MODEL 파일에 public $incrementing = false; false로 수정하였다. 
    ![image](https://user-images.githubusercontent.com/85022962/222957255-e19592ff-e177-4b54-9143-73493ca891b4.png)

    ![image](https://user-images.githubusercontent.com/85022962/222957215-62c56662-ac9e-4752-b253-75fae4d576ff.png)

    ![image](https://user-images.githubusercontent.com/85022962/222957204-6f5256e0-c2d5-4824-a798-0f61182dc9af.png)

