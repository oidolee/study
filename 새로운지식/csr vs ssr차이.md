# csr은 클라이언트(고객)컴퓨터에서 작업이 진행되어 고객 컴퓨터 사양에 따라 편차가 있을 수 있다.
## -ssr은 서버측에서 만들어서 전달하기에 csr에 단점을 극복 할 수 있다.
## - spa는 Open Graph Tag(op태그)링크보가, 미리보기가 안보여짐(하나의 페이지이기 때문에)

# 하지만 ssr일 때는 이러한 단점이 극복 되어 진다.

# ssr단점 => Node.js 및 서버쪽 이해가 필요 + Node.js 때문에 beforeCreate 와 Create에서 
window나 document 객체 접근이 불가능하다
