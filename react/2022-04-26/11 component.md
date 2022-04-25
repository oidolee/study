class 컴포넌트 이름 extends Component{
  render(){
    retrun();
  }
}
기본 컴포넌트 문법/ 컴포넌트 이름은 대문자 시작

class Subject extends Component{
  render(){
    retrun(
      <header>
          <h1>Title<h1>
          Hello world!!!
      </header>
    );
  }
}

Subject 컴포넌트 생성 후 
아래 App 컴포넌트에 넣어줌(App컴포넌트는 App.js->index.js->index.html)즉 최종 구현 입력 부분
            
class App extends Component{
  render(){
    retrun(
      <div className="App">
          <Subject></Subject>
      </div>
    );
  }
}
