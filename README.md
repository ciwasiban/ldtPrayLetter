# ldtPrayLetter
- A tool to send LDT pray letters.
- Running on Mac.
- Using PHPMailer class with google smtp to send email.

## reference
- ref:0 https://github.com/Synchro/PHPMailer
- ref:1 http://blog.e-happy.com.tw/php-使用phpmailer線上發信通過驗證的smtp/
- ref:2 https://stackoverflow.max-everyday.com/2017/12/php-phpmailer-smtp/
- ref:3 http://blog.e-happy.com.tw/php-使用phpmailer利用-gmail-的smtp-發信/
- ref:4 https://blog.csdn.net/Qyee16/article/details/72799852  ( mac 安裝openssl)

## Installation & loading
step1. clone this git:
```sh
git clone git@github.com:ciwasiban/ldtPrayLetter.git
```

step2. at top folder to run:
```sh
composer require phpmailer/phpmailer
```
(ref:2 or ref:1)
notice: PHP OpenSSL required (ref:4 or ref:3)

step3. 申請一個專門用來寄信的 google email 並且 降低其安全性設定 (ref:3)

step4. 資料設定
```sh
vim PrayLetter.php
```

step5. 下載 google sheet  檔案另存為 tsv file  取代 recipentList.tsv  的內容

step6. 開始寄信 run script
```php
php send.php
```
