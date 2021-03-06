# Over The Wire - Bandit

## Level 0

*  ssh bandit0@bandit.labs.overthewire.org
*  ls
*  cat readme
  *  boJ9jbbUNNfktd78OOpsqOltutMc3MY1

## Level 1

*  ssh bandit1@bandit.labs.overthewire.org
*  ls
*  cat ./-
  *  CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

## Level 2

*  ssh bandit2@bandit.labs.overthewire.org
*  ls
*  cat "spaces in this filename" 
  *  UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

## Level 3

*  ssh bandit3@bandit.labs.overthewire.org
*  ls
*  cd inhere
*  ls -al
*  cat .hidden
  *  pIwrPrtPN36QITSp3EQaw936yaFoFgAB

## Level 4

*  ssh bandit4@bandit.labs.overthewire.org
*  ls
*  cd inhere
*  ls -al
*  find . -type f | xargs file | grep text
*  strings ./-file07
  *  koReBOKuIDDepwhWk7jZC0RTdopnAYKh

## Level 5

*  ssh bandit5@bandit.labs.overthewire.org
*  find . -type f -readable -size 1033c ! -executable
  *  "inhere" is the directory
  *  "! -executable" specifies not executable
  *  "-type f" means find type is regular file
  *  "-size 1033c" says size of 1033 bytes
  *  "-readable" means read human-readable
*  cat "inhere/maybehere07/.file2"
  *  DXjZPULLxYr17uwoI01bNLQbtFemEgo7

## Level 6

*  ssh bandit6@bandit.labs.overthewire.org
*  cd ..
*  cat `find . -size 33c -user bandit7 -group bandit6 2>&1 | grep -v -e "Permission denied" -e "No such file or directory"`
  *  "cat `<stuff>`" uses the stuff inside `` for cat
  *  "-size 33c" for 33 bytes
  *  "-user bandit7" only files who the user is bandit7
  *  "-group bandit6" only files of the group bandit6
  *  "2>&1" reroutes stderr to stdout
  *  "| grep" pipe the output into grep
  *  "-v" invert search terms
  *  "-e "Permission denied" -e "No such file or directory"" searching on multiple terms
  *  Key: 
    *  HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

## Level 7

*  ssh bandit7@bandit.labs.overthewire.org
*  grep "millionth" data.txt 
  *  "millionth" word to search by
  *  "data.txt" file to search
  *  Key:
    *  cvX2JJa4CFALtqS87jk27qwqGhBM9plV

## Level 8

*  ssh bandit8@bandit.labs.overthewire.org
*  sort data.txt | uniq -u
  *  "sort data.txt" sort the file so that it is in order
  *  "uniq -u" print lines that are only appear once (needs to be ordered first)
  *  Key:
    *  UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

## Level 9

*  ssh bandit9@bandit.labs.overthewire.org
*  strings data.txt | grep "====" 
  *  "strings data.txt" gets all strings
  *  "grep "===="" Find strings begining with that
  *  Key:
    *  truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

## Level 10

*  ssh bandit10@bandit.labs.overthewire.org
*  base64 data.txt -d
  *  Decode base 64 data
  *  Key:
    *  IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

## Level 11

*  ssh bandit11@bandit.labs.overthewire.org
*  tr '[A-Za-z]' '[N-ZA-Mn-za-m]' < data.txt 
  *  tr translates or deletes caracters
  *  "[A-Za-z]" inital characters
  *  "[N-ZA-Mn-za-m]" what to map to
  *  "< data.txt " use data.txt as stdin
  *  Key:
    *  5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

## Level 12

*  ssh bandit12@bandit.labs.overthewire.org
*  mkdir /tmp/dc123
*  cp data.txt /tmp/dc123
*  cd /tmp/dc123
*  DECOMPRESSION TIME
  *  Lots of:
    *  gzip -d fileName
    *  tar -xvf fileName
    *  bzip2 -d fileName
    *  file fileName
    *  mv fileName fileName.gz
*  cat data8
  *  Key:
    *  8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

## Level 13

*  ssh bandit13@bandit.labs.overthewire.org
*  Copy and paste the sshkey.private file to your local computer
*  ssh bandit14@bandit.labs.overthewire.org -i sshkey.private 
    *  "-i" specifies file to use as rsa key
  *  Key:
    *  4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e


## Level 14

*  ssh bandit14@bandit.labs.overthewire.org
*  nc 127.0.0.1 30000
  * nc connects to a host
  * 127.0.0.1 is the local host
  * 30000 is the port
*  4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
  *  Key:
    *  BfMYroe26WYalil77FoDi9qh59eK5xNr

## Level 15

*  ssh bandit15@bandit.labs.overthewire.org
*  openssl s_client -connect localhost:30001 -ign_eof
  *  Key:
    *  cluFn7wTiGryunymYOu4RcffSxQluehd

## Level 16

*  ssh bandit16@bandit.labs.overthewire.org
*  nmap localhost -pS31000-32000
*  openssl s_client -ign_eof -connect localhost:31790
  *  We get a private ssh key

## Level 17

*  ssh bandit17@bandit.labs.overthewire.org -i bandit16.private
*  diff passwords.new passwords.old 
  * Key:
    * kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd

## Level 18

*  ssh bandit18@bandit.labs.overthewire.org "bash --noprofile"
*  ls
*  cat readme
  * Key:
    * IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x

## Level 19

*  ssh bandit19@bandit.labs.overthewire.org
*  ./bandit20-do euid=11020 cat /etc/bandit_pass/bandit20
  *  Key:
    *  GbKksEFF4yrVs6il55v6gwY5aVje5f0j

## Level 20

*  ssh bandit20@bandit.labs.overthewire.org
*  In session 1:
  *  echo "GbKksEFF4yrVs6il55v6gwY5aVje5f0j" | nc -l 2999
*  In session 2:
  *  ./suconnect 2999
* In session 1:
  *  "gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr" will be printed
  *  Key:
    *  gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr
    
## Level 21

*  ssh bandit21@bandit.labs.overthewire.org
*  cat /etc/cron.d/cronjob_bandit22
*  cat /usr/bin/cronjob_bandit22.sh 
*  cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
  *  Key:
    * Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI

## Level 22

*  ssh bandit22@bandit.labs.overthewire.org
*  cat /etc/cron.d/cronjob_bandit23
*  less /usr/bin/cronjob_bandit23.sh 
*  echo I am user bandit23 | md5sum | cut -d ' ' -f 1
*  cat /tmp/8ca319486bfbbc3663ea0fbe81326349
  *  Key:
    * jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n

## Level 23

*  ssh bandit23@bandit.labs.overthewire.org
*  cat /etc/cron.d/cronjob_bandit24
*  cat /usr/bin/cronjob_bandit24.sh 
*  cd /var/spool/bandit24
*  nano test.sh
```
myname=$(whoami)

cat /etc/bandit_pass/$myname > /tmp/1234567890bob.txt
```
*  chmod 777 test.sh
*  cat /tmp/1234567890bob.txt
  *  Key:
    * UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ

## Level 24

*  ssh bandit24@bandit.labs.overthewire.org
*  cd /tmp/directory12/
*  nano file.py
*  Paste bruteforce.py
*  python3 file.py
  *  Key:
    *  uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG

## Level 25

*  ssh bandit25@bandit.labs.overthewire.org
