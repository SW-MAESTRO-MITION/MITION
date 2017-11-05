# API

## USER

### 거래 주체 등록
- method: post
- body: name, email, phone_number
- url: user/signup_user
- response: USER object

### 거래 주체 정보 가져오기
- method: get
- param: user_id
- url: user/:id
- response: USER object

## ITEM

### 거래 물품 및 수량 등록
- method: post
- body: item_type, item_name, item_count
- url: user/signup_item
- response: ITEM object
 
## CONTRACT

### 계약 정보 가져오기
- method: get
- param: resident_user_id
- url: contract/user/:id
- response: CONTRACT object
