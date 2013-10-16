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








