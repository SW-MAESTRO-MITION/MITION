# API

## USER

### 회원가입 (createUser)
- method: post
- body: name, email, password
- url: /user
- response: USER object

### 로그인 (getUser)
- method: get
- params: id
- url: /user/:id
- response: USER object

### 회원정보수정 (modifyUser)
- method: put
- params: id
- url: /user/:id
- response: USER object

### 회원탈퇴 (deleteUser)
- method: delete
- params: id
- url: /user/:id
- response: USER object


## CONTRACT

### 계약 등록 (addContract)
- method: post
- body: date, hash, name
- url: /contract/add

### 계약 찾기 (findContract)
- method: get
- param: hash
- url: /find/:hash
- response: CONTRACT object
