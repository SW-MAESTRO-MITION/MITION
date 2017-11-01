# Model

## User 
- 사용자 정보

### name
- 사용자 이름
- 자료형 : string
- 입력 필수

### email
- 이메일 주소 (로그인 아이디)
- 자료형 : string
- 입력 필수

### password
- 비밀번호
- 자료형 : string
- 입력 필수

### id_number
- 주민등록번호
- 자료형 : int
- 입력 필수

### phone_number
- 전화번호
- 자료형 : string
- 입력 필수

----------------------

## Contract 
- 계약 정보

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
- 입력 필수
- 기본값 : 0

### admin_sign_image_url
- 매도인 서명 이미지 주소
- 자료형 : string
- 입력 필수

### guest_sign_image_url
- 매수인 서명 이미지 주소
- 자료형 : string
- 입력 필수

### pdf_url
- 최종 계약서 pdf 해쉬값
- 자료형 : string
- 입력 필수

## Real Estate Contract
- 
### contract_id
- 계약 종류 식별자 (부동산 계약, 중고자 계약, ...)
- 자료형 : string
- 입력 필수

----------------------

## real_estate_type

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

###	"mid_price": {
- 중도금 
- 자료형 : int
- 입력 선택
- 기본값 : 0

###	final_price
- 잔금
- 자료형 : int
- default : 0
- 입력 선택

###	month_money
- 월세금
- 자료형 : int
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
- 자료형 : string
- 입력 선택

###	duration
- 계약 기간
- 자료형 : string
- 입력 필수

###	extra_condition
- 특약사항
- 자료형 : string 배열
- 입력 선택