# CMS451-InfoSec

midterm prep
bandit.labs.overthewire.org
port:2020
ssh bandit(nomre)@bandit.labs.overthewire.org -p 2220 (Git bashden)




bandit0:bandit0
ls
cat readme


bandit1: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
ls
faylin adinda - var:
cat ./-

bandit2: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx
bandit2@bandit:~$ cat ./--spaces\ in\ this\ filename--




bandit3: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
gizli fayl:
cd inhere
ls -a




bandit4: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
human-readable:
file ./-file*
cat ./-file07




bandit5:4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
human-readable
1033 bytes in size
not executable
:
bandit5@bandit:~/inhere$ find . -readable -size 1033c
ya da :
find . -type f -readable -size 1033x ! -executable

cat ./maybehere07/.file2





bandit6: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
owned by user bandit7
owned by group bandit6
33 bytes in size
bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c
min dene sey cixacaq
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password




bandit7:morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
in the file data.txt next to the word millionth
cat data.txt | grep "millionth"




bandit8: dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
cat data.txt | sort | uniq -c
ya da: 
cat data.txt | sort | uniq -u



bandit9: 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.
bandit9@bandit:~$ strings data.txt | grep "=="



bandit10:FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
in the file data.txt, which contains base64 encoded data
bandit10@bandit:~$ base64 -d data.txt




bandit11: dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
cat data.txt 
-> rot13.com -> decode




bandit12: 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
bandit12@bandit:~$ mkdir /tmp/shahin
bandit12@bandit:~$ cd /tmp/shahin
bandit12@bandit:/tmp/shahin$ cp ~/data.txt .
bandit12@bandit:/tmp/shahin$ ls
hexdumpdan coxar: 
bandit12@bandit:/tmp/shaka$ xxd -r data.txt > data
bandit12@bandit:/tmp/shahin$ file data
gzip idi ona gore:
mv data data.gz 
file data
bzip2:
mv data data.bz2


bandit12@bandit:/tmp/shahin$ mv data5.bin data5.tar
bandit12@bandit:/tmp/shahin$ tar -xf data5.tar
bandit12@bandit:/tmp/shahin$ bunzip2 data6.bz2
bandit12@bandit:/tmp/shahin$ gunzip data8.gz




bandit13: FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn
cat sshkey.private
local
$ ssh -i /c/ShahinGanbar/InfoSec/sshkey.private bandit14@bandit.labs.overthewire.org -p 2220

bandit14@bandit:~$ cat /etc/bandit_pass/bandit14





bandit14: MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS
port 30000 on localhost'a passwordu submit et dedi
bandit14@a:~$ printf "%s\n" "MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS" | nc localhost 30000
Correct!
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo




bandit15: 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
SSL/TLS istedi:
bandit15@bandit:~$ openssl s_client -connect localhost:30001
paste the password of bandit15




bandit16: kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx
port range var
bandit15@bandit:~$ nmap localhost -p 31000-32000
portlari yaziriq bir bir kodu yapisdiririq her defesinde
bandit15@bandit:~$ openssl s_client -connect localhost:31046 -quiet

rsa key seklinde verilmisdi,faylin icinde qoyub git bashde yaziriq:
chmod 600 /c/ShahinGanbar/InfoSec/ssh17key.private
ssh -i ssh17key.private bandit17@bandit.labs.overthewire.org -p 2220
cat /etc/bandit_pass/bandit17




bandit17: EReVavePLFHtFlFsjn3hyzMlvSuSAcRD
bandit17@bandit:~$ diff passwords.old passwords.new




bandit18:x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
acir readme'ni kodu gosterir sonra atir:
$ ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme




bandit19: cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8
setuid: ozunu bandit 20 kimi aparib kodu goturursen
./bandit20-do cat /etc/bandit_pass/bandit20 (faylin adindan evvel ./ yaz)




bandit20: 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
2 dene gitbash ac ikisinde de bandit 20ye qosul:
ssh bandit20@bandit.labs.overthewire.org -p 2220
sonra birinci tabda bunu yaz(dirnaqin icinde bandit20nin kodu):
echo -n '0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO' | nc -l -p 9009 &
sonra ikinci tabda bunu yaz(eyni port nomresi ile):
./suconnect 9009
sonra gonderir kodu birinci taba




bandit21: EeoULMCra2q0dSkYj561DX7s1CpBuOBt
cron vaxt temasi:
cd /etc/cron.d/ 
ll
cat cronjob_bandit22
directoryni kopyala: /usr/bin/cronjob_bandit22.sh
cat /usr/bin/cronjob_bandit22.sh
sonra bele birsey cixacaq kopyala onu yaz basqa yere(
#!/bin/bash
chmod 644 /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
cat /etc/bandit_pass/bandit22 > /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
bandit21@bandit:/etc/cron.d$ )


mkdir /tmp/shahin
cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv > /tmp/shahin/temp
cat /tmp/shahin/temp
kodu gotur fso



bandit 22: tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q
yene cron temasi:
bandit22ye gir
cd /etc/cron.d/
ll
cat cronjob_bandit23
kopyala yuxaridakini: /usr/bin/cronjob_bandit23.sh 
cat /usr/bin/cronjob_bandit23.sh

sonra bele birsey cixacaq kopyala onu yaz basqa yere(
#!/bin/bash

myname=$(whoami) 
mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)

echo "Copying passwordfile /etc/bandit_pass/$myname to /tmp/$mytarget"

cat /etc/bandit_pass/$myname > /tmp/$mytarget
)


burada myname = bandit23
mytargeti tapmaq ucun bunu run ele(bandit22ni $myname yerine) : 
echo I am user bandit23 | md5sum | cut -d ' ' -f 1

mytargeti gotur: 8ca319486bfbbc3663ea0fbe81326349

mkdir /tmp/shahin2
cat /tmp/8ca319486bfbbc3663ea0fbe81326349 > /tmp/shahin3/temp
cat  /tmp/shahin2/temp


bandit23: 0Zf11ioIjMVN551jX3CmStKLYqjk54Ga
yene cron temasi:
bandit23e gir
cd /etc/cron.d/
ll
cat cronjob_bandit24
kopyala yuxaridakini:  /usr/bin/cronjob_bandit24.sh
cat /usr/bin/cronjob_bandit24.sh
kod cixacaq basqa yere yaz rahat olsun: (
#!/bin/bash

myname=$(whoami)

cd /var/spool/$myname/foo    
echo "Executing and deleting all scripts in /var/spool/$myname/foo:"
for i in * .*;
do
    if [ "$i" != "." -a "$i" != ".." ];
    then
        echo "Handling $i"
        owner="$(stat --format "%U" ./$i)"
        if [ "${owner}" = "bandit23" ]; then
            timeout -s 9 60 ./$i
        fi
        rm -f ./$i
    fi
done

)

sonra:
cd /var/spool/bandit24/foo ele
myname=bandit24 ele
ar/spool/bandit24/foo ele

then:

mkdir /tmp/shahin4
chmod 777 -R /tmp/shahin4
cat > /tmp/shahin4/script.sh
#!/bin/bash
cat /etc/bandit_pass/bandit24 > /tmp/shahin4/password
cp /tmp/shahin4/script.sh /var/spool/bandit24/foo
cat /tmp/shahin4/password

chmod 777 -R /tmp/shahin4 
cp /tmp/shahin4/script.sh /var/spool/bandit24/foo
cat /tmp/shahin4/password

ll /tmp/shahin4(yoxlamaq ucun )


bandit 24: gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8