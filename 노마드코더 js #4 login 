# 4.0 Input Values

## 배운 내용

HTML의 input에 사용자가 입력한 값을 JavaScript에서 가져오는 방법

`querySelector()`를 이용한 HTML 요소 선택과
input의 `value`를 이용한 입력값 확인

```js
const loginInput = document.querySelector("#login-form input");
const loginButton = document.querySelector("#login-form button");
```

```html
<div id="login-form">
	<input type="text" placeholder="What is your name?" />
	<button>Log In</button>
</div>
```


### 핵심 정리

* `querySelector()` : 원하는 HTML 요소 선택
* `value` : input에 입력된 값 확인

# 4.1 Form Submission

## 배운 내용

username이 비어있거나 너무 길면 안되는 조건 js

```js
function onLoginBtnClick(){
	const username = loginInput.value;
	if (username === ""){
		alert("Please write your name")
	} else if (username.length > 15){
		alert("Your name is too long")
	}
}

```

username이 비어있거나 너무 길면 안되는 조건 html
```html
<form id="login-form">
	<input
		required
		maxlength = "15"
		type = "text"
		placeholder = "What is your name?"
	/>
</form>
```


# 4.2 Events

## 배운 내용

JavaScript에서 이벤트를 감지하고 처리하는 방법

`addEventListener()`를 이용한 이벤트 감지와 함수 실행

```js
loginForm.addEventListener("submit", onLoginSubmit);
```

이벤트가 발생했을 때 함수에 이벤트 객체를 전달하는 방법

```js
function onLoginSubmit(event) {
    console.log(event);
}
```

### 핵심 정리

이벤트 발생
→ `addEventListener()`를 통한 이벤트 감지
→ 지정한 함수 실행
→ 이벤트 객체를 이용한 이벤트 처리

# 4.3 Events part Two

## 배운 내용

이벤트 객체와 `preventDefault()`를 이용한
브라우저의 기본 동작 제어

```js
function onLoginSubmit(event) {
    event.preventDefault();
}
```

`event`를 이용한 이벤트 정보 확인과
`preventDefault()`를 이용한 기본 동작 방지

### 핵심 정리

이벤트 발생
→ `addEventListener()`를 통한 이벤트 감지
→ 함수 실행
→ `event`를 이용한 이벤트 처리

# 4.4 Getting Username

## 배운 내용

input에 사용자가 입력한 username을 가져오는 방법

input의 `value`를 변수에 저장하여
JavaScript에서 입력값을 사용하는 과정

```js
const username = loginInput.value;
```

### 핵심 정리

사용자가 username 입력
→ `input.value`로 값 가져오기
→ 변수에 저장
→ JavaScript에서 사용

# 4.5 Saving Username

## 배운 내용

JavaScript의 변수에 저장된 값과
브라우저에 데이터를 저장하는 방법의 차이

브라우저에 데이터를 저장하기 위한 `localStorage` 사용

```js
localStorage.setItem("username", username);
```

`setItem()`을 이용한 key와 value 형태의 데이터 저장

### 핵심 정리

* `localStorage` : 브라우저에 데이터를 저장하는 공간
* `setItem()` : 데이터 저장

```js
localStorage.setItem("key", "value");
```

# 4.6 Loading Username

## 배운 내용

`localStorage`에 저장한 데이터를 다시 가져오는 방법

`getItem()`을 이용한 저장 데이터 불러오기

```js
const savedUsername = localStorage.getItem("username");
```

### 핵심 정리

데이터 저장

```js
localStorage.setItem("username", username);
```

데이터 불러오기

```js
localStorage.getItem("username");
```

# 4.7 Super Recap

## 전체 내용 정리

username을 입력받고
form의 이벤트를 처리한 뒤
username을 저장하고 다시 불러오는 전체 과정

### 전체 과정

username 입력
→ input의 `value` 가져오기
→ form의 `submit` 이벤트 발생
→ `preventDefault()`로 기본 동작 제어
→ username 저장
→ `localStorage`에 저장
→ 저장된 username 불러오기
→ 화면에 username 표시

### 배운 내용

* `querySelector()` : HTML 요소 선택
* `value` : input의 입력값 확인
* `addEventListener()` : 이벤트 감지
* `submit` : form 제출 이벤트
* `event` : 발생한 이벤트 정보
* `preventDefault()` : 기본 동작 방지
* `localStorage` : 브라우저 데이터 저장
* `setItem()` : 데이터 저장
* `getItem()` : 데이터 불러오기


