# Login System
>Made by: 000hen <br/>
>Version: 1 <br/>
>Copyright: 3ZH-Studio <br/>

This is a login system use PHP

## How To Use

First, add new databases in your MySQL server
![db](/img/n1.png)

Second, add user (password need encrypt with MD5)

Next, change code in the "config.php"

```php
$dbhost="localhost"; //填入資料庫位置
$dbuser="root"; //填入資料庫名稱
$dbpass="12345" //填入資料庫密碼(是'dbuser'的密碼)
$dbselect="login_sys"; //選擇資料庫
$dbtable="login"; //填入資料"表"
```

And, add others file you need add code:
```php
require_once($_SERVER['DOCUMENT_ROOT'].'/admin/page/flf.php');

if (@$login == "1"){
  //Code Here!
}else{
	header("location: //".$_SERVER['DOCUMENT_ROOT']."/admin/login.php?return=$url");
}
```
