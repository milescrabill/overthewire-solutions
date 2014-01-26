Bandit Solutions
==================
[http://www.overthewire.org/wargames/bandit/](http://www.overthewire.org/wargames/bandit/)

Level 0
--------
```
ssh bandit0@bandit.labs.overthewire.org
```

pass is `bandit0`

```
cat readme
```

Level 1
---------
```
ssh bandit1@bandit.labs.overthewire.org
```

pass is `boJ9jbbUNNfktd78OOpsqOltutMc3MY1`

```
cat ./-
```

Level 2
--------
```
ssh bandit2@bandit.labs.overthewire.org
```

pass is `CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9`

```
cat spaces\ in\ this\ filename
```

Level 3
-------
```
ssh bandit3@bandit.labs.overthewire.org
```

pass is `UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK`

```
cd inhere
ls -a
cat .hidden
```

Level 4
-------
```
ssh bandit4@bandit.labs.overthewire.org
```

pass is `pIwrPrtPN36QITSp3EQaw936yaFoFgAB`

```
cd inhere
ls
for file in *; do echo $file; cat ./$file; done
cat ./-file07
```

Level 5
-------
```
ssh bandit5@bandit.labs.overthewire.org
```

pass is `koReBOKuIDDepwhWk7jZC0RTdopnAYKh`

```
cd inhere
for file in `find -size 1033c -perm -a-x`; do file -b $file | grep text &>/dev/null && echo $file; done 
cat ./maybehere07/.file2
```

Level 6
-------
```
ssh bandit6@bandit.labs.overthewire.org
```

pass is `DXjZPULLxYr17uwoI01bNLQbtFemEgo7`

```
find / -group bandit6 -user bandit7 -type f -size 33c 2> /dev/null
cat /var/lib/dpkg/info/bandit7.password
```

Level 7
-------
```
ssh bandit7@bandit.labs.overthewire.org
```

pass is `HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs`

```
cat data.txt | grep millionth
```

Level 8
-------
```
ssh bandit8@bandit.labs.overthewire.org
```

pass is `cvX2JJa4CFALtqS87jk27qwqGhBM9plV`

```
sort data.txt | uniq -u
```

Level 9
-------
```
ssh bandit9@bandit.labs.overthewire.org
```

pass is `UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR`

```
strings data.txt | grep =
```

Level 10
--------
```
ssh bandit10@bandit.labs.overthewire.org
```

pass is `truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk`

```
base64 -d -i data.txt 
```

Level 11
--------
```
ssh bandit11@bandit.labs.overthewire.org
```

pass is `IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR`

```
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

Level 12
--------
```
ssh bandit12@bandit.labs.overthewire.org
```

pass is `5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu`

```
xxd -r data.txt > data.bin
file data.bin
mv data.bin data.gz
gzip -d data.gz
file data
mv data data.bz2
bzip2 -d data.bz2
file data
mv data data.gz
gzip -d data.gz 
file data
tar -xvf data
file data5.bin
tar -xvf data5.bin
bzip2 -d data6.bin
file data6.bin.out
tar -xvf data6.bin.out
file data8.bin
mv data8.bin data8.gz
gzip -d data8.gz
file data8
cat data8
```

Level 13
```
ssh bandit13@bandit.labs.overthewire.org
```

pass is `8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL`

```
ssh bandit14@localhost -i sshkey.private
cat /etc/bandit_pass/bandit14
```

Level 14
```
ssh bandit14@bandit.labs.overthewire.org
```

pass is `4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e`

```
cat /etc/bandit_pass/bandit14 | nc localhost 30000
```

Level 15
```
ssh bandit15@bandit.labs.overthewire.org
```

pass is `BfMYroe26WYalil77FoDi9qh59eK5xNr`

```
ncat --ssl localhost 30001
# (paste the password for this leve)
```


Level 16
```
ssh bandit16@bandit.labs.overthewire.org
```

pass is `cluFn7wTiGryunymYOu4RcffSxQluehd`

```
nmap -p31000-32000 localhost
echo "cluFn7wTiGryunymYOu4RcffSxQluehd" | ncat --ssl localhost 31046 # nope
echo "cluFn7wTiGryunymYOu4RcffSxQluehd" | ncat --ssl localhost 31518 # nope
echo "cluFn7wTiGryunymYOu4RcffSxQluehd" | ncat --ssl localhost 31691 # nope
echo "cluFn7wTiGryunymYOu4RcffSxQluehd" | ncat --ssl localhost 31790 # bingo
# copy the ssh key to clipboard
cat > /tmp/foobar9001.key
# paste the ssh key, ctrl+d
chmod 600 /tmp/foobar9001.key
ssh bandit17@localhost -i /tmp/foobar9001.key
cat /etc/bandit_pass/bandit17
```

Level 17
```
ssh bandit17@bandit.labs.overthewire.org
```

pass is `xLYVMN9WE5zQ5vHacb0sZEVqbrp7nBTn`

```
diff passwords.old passwords.new
```

Level 18
```
ssh bandit18@bandit.labs.overthewire.org
```

pass is `kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd`

```
ssh bandit18@bandit.labs.overthewire.org # nope
ssh -t bandit18@bandit.labs.overthewire.org /bin/sh
cat readme 
```

Level 19
```
ssh bandit19@bandit.labs.overthewire.org
```

pass is `IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x`

```
./bandit20-do cat /etc/bandit_pass/bandit20
```

Level 20
```
ssh bandit20@bandit.labs.overthewire.org
```

pass is `GbKksEFF4yrVs6il55v6gwY5aVje5f0j`

```
nc -l 9001 < /etc/bandit_pass/bandit20 &
./suconnect 9001
```

Level 21
```
ssh bandit21@bandit.labs.overthewire.org
```

pass is `gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr`

```
ls /etc/cron.d/
cat /etc/cron.d/cronjob_bandit22
cat /usr/bin/cronjob_bandit22.sh
cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
```

Level 22
```
ssh bandit22@bandit.labs.overthewire.org
```

pass is `Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI`

```
cat /etc/cron.d/cronjob_bandit23
cat /usr/bin/cronjob_bandit23.sh
myname='bandit23'
mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)
cat /tmp/$mytarget
```

Level 23
```
ssh bandit23@bandit.labs.overthewire.org
```

pass is `jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n`

```
cat /etc/cron.d/cronjob_bandit24
cat /usr/bin/cronjob_bandit24.sh
echo "cat /etc/bandit_pass/bandit24 > /tmp/over9000.txt && chmod 777 /tmp/over9000.txt" > /var/spool/bandit24/foobar.sh
```


