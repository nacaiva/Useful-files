# Bandit wargame

## Level 0-->Level 1
The password for the next level is stored in a file called - located in the home directory
```
ssh bandit0@bandit.labs.overthewire.org
pass: bandit0
ls
cat readme
```
boJ9jbbUNNfktd78OOpsqOltutMc3MY1

## Level 1-->Level 2
The password for the next level is stored in a file called spaces in this filename located in the home directory
```
ssh bandit1@bandit.labs.overthewire.org
pass: boJ9jbbUNNfktd78OOpsqOltutMc3MY1
ls
cat ./-
```
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

## Level 2-->Level 3
The password for the next level is stored in a file called spaces in this filename located in the home directory
```
ssh bandit2@bandit.labs.overthewire.org
pass:CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
ls
cat 'spaces in this filename'
```
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

## Level 3-->Level 4
The password for the next level is stored in a hidden file in the inhere directory.
```
ssh bandit3@bandit.labs.overthewire.org
pass: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
ls
cd inhere
ls -lah
cat .hidden
```
pIwrPrtPN36QITSp3EQaw936yaFoFgAB

## Level 4-->Level 5
The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

```
ssh bandit4@bandit.labs.overthewire.org
pass:pIwrPrtPN36QITSp3EQaw936yaFoFgAB
ls
cd inhere
ls
cd ./-file07
```
koReBOKuIDDepwhWk7jZC0RTdopnAYKh

## Level 5-->Level 6
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties: - human-readable - 1033 bytes in size - not executable
```
ssh bandit5@bandit.labs.overthewire.org
pass: koReBOKuIDDepwhWk7jZC0RTdopnAYKh
ls
cd inhere
find . -type f -size 1033c ! -executable
cat $(find . -type f -size 1033c ! -executable)
```
DXjZPULLxYr17uwoI01bNLQbtFemEgo7

## Level 6--> Level 7
The password for the next level is stored somewhere on the server and has all of the following properties: - owned by user bandit7 - owned by group bandit6 - 33 bytes in size
```
ssh bandit6@bandit.labs.overthewire.org
pass: DXjZPULLxYr17uwoI01bNLQbtFemEgo7
cat $(find / -size 33c -group bandit6 -user bandit7)
```
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

##Level 7--> Level 8
The password for the next level is stored in the file data.txt next to the word millionth
```
ssh bandit7@bandit.labs.overthewire.org
pass: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
```
