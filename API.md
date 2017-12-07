# API

## USER

### createUser
- method: post
- body: name, email, password
- url: /user
- response: USER object

### getUser
- method: get
- params: id
- url: /user/:id
- response: USER object

### login
- method: post
- body: email, password
- url: /user/login
- response: USER object

### modifyUser
- method: put
- params: id
- url: /user/:id
- response: USER object

### deleteUser
- method: delete
- params: id
- url: /user/:id
- response: USER object


## CONTRACT

### addContract
- method: post
- body: date, hash, name
- url: /contract/add

### findContract
- method: get
- param: hash
- url: /find/:hash
- response: CONTRACT object


## FILE

### uploadFile
- method: post
- file: path, originalname, size
- url: /file/upload


## MAILING

### sendMail
- method: post
- body: hostmail, guestmail
- url: /mailing


## TRANSACTION

### createTransaction
- method: post
- body: sender_name, sender, recipient, absolute_path, file_name, date
- url: /transaction
- response: TRANSACTION object

### getSenderTransaction
- methond: get
- params: id
- url: /transaction/sender/:id
- response: TRANSACTION object

### getRecipientTransaction
- method: get
- params: id
- url: /transaction/recipient/:id
- response: TRANSACTION object

### acceptTransaction
- method: post
- params: id
- url: /transaction/accept/:id
- response: TRANSACTION object
