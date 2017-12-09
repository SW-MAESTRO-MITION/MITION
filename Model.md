# Model

## user
- name
  - type: string
  - required: true
- email
  - type: string
  - required: true
- password
  - type: string
  - required: true
- address
  - type: string
- transaction_id
  - type: string
- type_of_party
  - type: string
- is_checked_registered_contract
  - type: boolean
  - default: true

## registeredTransaction

- email
  - type: string
  - required: true

- path
  - type: string
  - required: true

## transaction

- sender_name
  - type: string
  - required: true

- sender
  - type: string
  - required: true

- recipient
  - type: string
  - required: true

- path
  - type: string
  - required: true

- file_name
  - type: string
  - required: true

- transaction_date
  - type: string
  - required: true
