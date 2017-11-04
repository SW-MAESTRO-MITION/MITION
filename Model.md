# Model

## User 
- 거래 주체

### name
- 거래 주체 이름
- 자료형 : string
- 입력 필수

### email
- 이메일 주소
- 자료형 : string
- 입력 필수

### phone_number
- 전화번호
- 자료형 : string
- 입력 필수

----------------------

## Item
- 거래 물품

### item_type
- 거래 물품 종류 (부동산, 비상장 주식, 중고차 매매, 자리 예약, ...)
- 자료형 : int
- 입력 필수

### item_name
- 거래 물품 이름
- 자료형 : string
- 입력 필수

### item_count
- 거래 물품 수량
- 자료형 : int
- 입력 필수

### item_id
- 거래 물품 아이디
- 자료형 : int
- 입력 필수

----------------------

## Contract 
- 계약서

### admin_id
- 매도인 식별자
- 자료형 : string
- 입력 필수

### guest_id
- 매수인 식별자
- 자료형 : string
- 입력 필수

### date
- 계약 일자
- 자료형 : string
- 입력 필수

### contract_type
- 계약 종류 식별자 (부동산 계약, 중고자 계약, ...)
- 자료형 : int
- 기본값 : 0
- 입력 필수

### admin_sign_image_url
- 매도인 서명 이미지 주소
- 자료형 : string
- 입력 필수

### guest_sign_image_url
- 매수인 서명 이미지 주소
- 자료형 : string
- 입력 필수

### pdf_url
- 최종 계약서 pdf 해쉬값 (주소)
- 자료형 : string
- 입력 필수

----------------------

## Real Estate Contract
- 부동산 계약 정보

###	contract_id
- 계약 식별자 
- 자료형 : string
- 입력 필수

###	real_estate_type
- 부동산 계약 종류 식별자 (매매, 전세, 월세 구분)
- 자료형 : int
- 입력 필수
		
###	contract_price
- 계약금
- 자료형 : int
- 입력 선택

###	mid_price
- 중도금 
- 자료형 : int
- 기본값 : 0
- 입력 선택

###	final_price
- 잔금
- 자료형 : int
- 기본값 : 0
- 입력 선택

###	month_money
- 월세금
- 자료형 : int
- 기본값 : 0
- 입력 선택

###	address
- 소재지
- 자료형 : string
- 입력 필수

###	land_type
- 토지 정보 : 지목
- 자료형 : string
- 입력 선택

###	land_size
- 토지 정보 : 면적
- 자료형 : number
- 기본값 : 0
- 입력 선택

###	building_struct
- 건물 정보 : 구조
- 자료형 : string
- 입력 선택

###	building_usage
- 건물 정보 : 용도
- 자료형 : string
- 입력 선택

###	building_size
- 건물 정보 : 면적
- 자료형 : number
- 기본값 : 0
- 입력 선택

###	duration
- 계약 기간
- 자료형 : string
- 입력 필수

###	extra_condition
- 특약사항
- 자료형 : string 배열
- 입력 선택