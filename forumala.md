## Formulas for google sheet 🧪
-----
### 1️⃣ The formula to generate consecutive code which is combination of letters and numbers

```
="QR"&ROW(A1)+1000
```
##### Output
| QR Key|
| ------|
| QR1001  | 
| QR1002  | 
| QR1002  | 

Replace "QR" and the number 1000 with your desired letters and number

eg.``` ="CODE"&ROW(A1)+154```

##### Output
| QR Key|
| ------|
| CODE155  | 
| CODE156  | 
| CODE157  | 

----
### 2️⃣ Formula to generate random code for qr code(More secure)
```
=CHAR(RANDBETWEEN(65,90))&CHAR(RANDBETWEEN(65,90))&CHAR(RANDBETWEEN(65,90))&CHAR(RANDBETWEEN(65,90))&CHAR(RANDBETWEEN(65,90))&RANDBETWEEN(10,99)
```
##### Output
| QR Key|
| ------|
| OJBXE36  | 
| LZGGR16  | 
| BDXHP18  | 
----
### 3️⃣ Formula to generate qr code image url
```
="https://chart.googleapis.com/chart?chs=300x300&cht=qr&chl="&ENCODEURL(A1)
```
##### Output
| QR Key	    | QR Key Url    |
| ------------- | ------------- |
| QR1001  | https://chart.googleapis.com/chart?chs=300x300&cht=qr&chl=QR1001  |
| QR1002  | https://chart.googleapis.com/chart?chs=300x300&cht=qr&chl=QR1002  |
| QR1003  | https://chart.googleapis.com/chart?chs=300x300&cht=qr&chl=QR1003  |

### 4️⃣ Formula to generate qr code image in google sheets
```
=image("https://chart.googleapis.com/chart?chs=300x300&cht=qr&chl="&ENCODEURL(A1))
```
Here "A1" is the column position
##### Output
![image](https://user-images.githubusercontent.com/105426078/231955886-3556eb7b-90c1-44f6-a7d9-dbeaed56c11b.png)

