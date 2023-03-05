@if ( auth()->user() )
   {{auth()->user()}}
   <h1 class="text-3xl text-center mt-20"></h1>
@endif
로그인 한 유저가 있을시 if구문 돌아감
