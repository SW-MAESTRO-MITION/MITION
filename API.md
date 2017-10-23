# API

> candidate_room을 dibs로 변경함. dibs = 찜하다.

## USER

### 유저 회원가입
- method: post
- body: name, password, email, phone_number
- url: user/sign
- response: USER object

### 유저 로그인
- method: post
- body: id, password
- url: user/login
- response: USER object

### 유저 정보 가져오기
- method: get
- param: user_id
- url: user/:id
- response: USER object

### 찜한 방 가져오기 (없어도 될 듯, 유저 데이터를 가져올 때 같이 날라옴.)
- method: get
- param: user_id
- url: user/:id/dibs
- response: USER object

### 방 찜하기
- method: put
- param: room_id
- url: user/dibs/:id/addtion
- response: USER object

### 방 찜하기 취소
- method: put
- param: room_id
- url: user/dibs/:id/extraction
- response: USER object
 
## CONTRACT

### 계약 정보 가져오기
- method: get
- param: resident_user_id
- url: contract/user/:id
- response: CONTRACT object

## ROOM

### 방 정보 가져오기
- method: get
- param: room_id
- url: room/:id
- response: ROOM object
