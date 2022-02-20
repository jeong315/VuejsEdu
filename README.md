

1. vue.js
  홈페이지: https://v2.vuejs.org/v2/guide/


2. Vue Router ( unpkg.com은 더 이상 지원 안함)
    홈페이지: https://v3.router.vuejs.org/guide
    
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/vue-router/dist/vue-router.js"></script>
    
    
    
3. axios
    홈페이지: https://github.com/axios/axios
 
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/axios/dist/axios.min.js"></script>
    
    *json 실습 사이트
    https://reqres.in/ 
    https://jsonplaceholder.typicode.com/
    http://www.kobis.or.kr/kobisopenapi/webservice/rest/boxoffice/searchDailyBoxOfficeList.json?key=3d430a039fb1bae3fe5f0bc48df64e46&targetDt=20120101
==>해당 날짜의 박스오피스
    
    *sts 및 postgres sql 프로그램
    https://drive.google.com/drive/folders/1gbYWWgKq6axNKs4BODZlsmzMs-sVzWAr?usp=sharing
  
  
4. vuex  
   홈페이지: https://v3.vuex.vuejs.org/kr/ 
 
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/vuex/dist/vuex.js"></script>

 5. vueCLI

  https://cli.vuejs.org/guide/installation.html

  npm install -g @vue/cli
  
  vue create 프로젝트명
-------------------------
vsc 확장자
- vetur
- live server
- vue2 snippet
- prettier
  ==> vsc , preference > settings > 검색:editor format 을 prettier - Code formatter 로
				  format on save 체크

크롬 확장프로그램 vue.js devtools 다운로드

* 파라미터 전송
1. path variable ( ==>RESTFul 서비스 방식)
    : http://localhost:5500/vuestudy/foo/넘겨줄파라미터값
    : http://localhost:5500/vuestudy/foo/park

    url 경로 ? foo/ 파라미터값 까지.

2. query string
    : http://localhost:5500/vuestudy/foo?key=value&key2=value2
    : http://localhost:5500/vuestudy/foo?id=park

    url 경로 ? /foo 까지.


path: query만 되고
name:은 params, query 다 된다고?
-----------------
///////////////////////////////////////////
클라이언트 			   서버
	      요청(비동기, ajax)
	        get: select   =======>@GetMapping
	        post: insert  =======>@PostMappin
	        put: update  =======>@PutMapping
	        delete: delete   =====>@DeleteMapping
	      파라미터 전달
	        - pathVariable ==> ~/vuejs/user/1234  ==> @PathVariable
	        - queryString  ==> ~/vuejs?user=1234& => @RequestParam
- vue.js기반 -----------------------> 
	   <----------------------
	       응답(data:JSON)

JSON 응답 서비스 제공하는 서버
    https://reqres.in/ ==> 내려서 get/post/put/delete 방식 있음. 눌러서 확인
    https://jsonplaceholder.typicode.com/ ==> get방식만 지원함

* 비동기 처리 
1) XMLHttpRequest 객체 (전통적인 자바스크립트 )
2) Promise 객체 ( ES6 )
3) axios 외부 라이브러리 ( Vuejs 표준 )

----------------------------------
///////////////////////////////////////
http://localhost:8076/ecommerce/customer/rest/customers
http://localhost:8076/ecommerce/customer/swagger-ui.html
----------------------------------
//////////////vuex/////////////////////////
* 컴포넌트간의 통신
1.부모/자식 형태의 레이아웃
부 --> 자 : props
자 --> 부 : 이벤트(커스텀 이벤트)
		커스텀 이벤트 생성: emit() 이용

2. 같은 레벨(형제)의 레이아웃
3. 이벤트 버스 이용 ( var eventBus = new Vew() );


