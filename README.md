# useful_regexp

## 이메일 체크
> !/^(([^<>()\[\]\.,;:\s@\"]+(\.[^<>()\[\]\.,;:\s@\"]+)*)|(\".+\"))@(([^<>()[\]\.,;:\s@\"]+\.)+[^<>()[\]\.,;:\s@\"]{2,})$/
<hr/>

## 비밀번호 체크 
- 영문,숫자,특수문자($@^!%*#?&)를 모두 포함하여 8자 이상
> !/^(?=.*[A-Za-z])(?=.*[0-9])(?=.*[$@^!%*#?&]).{8,50}$/
<hr/>

## 가격에 ',' 넣기

> /\B(?=(\d{3})+(?!\d))/g

ex) price.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ',')
<hr/>

