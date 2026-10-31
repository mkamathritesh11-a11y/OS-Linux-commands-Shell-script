# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
### Display the content of the files
cat < file1
## OUTPUT
<img width="692" height="162" alt="690438013-f7337cb5-ca7c-44ca-847d-292698f487f8" src="https://github.com/user-attachments/assets/5f7fde85-475c-4256-80a4-9c12b0686f93" />

<img width="691" height="115" alt="image" src="https://github.com/user-attachments/assets/d605a059-d8e1-46ca-acd2-2b1d23bf94e8" />

<img width="541" height="47" alt="690442440-daacc6fe-3cc5-4810-b1cd-d261af69eeea" src="https://github.com/user-attachments/assets/d5708a05-fc0a-4e61-a87d-5c385f6a919c" />

cat < file2
## OUTPUT
<img width="570" height="207" alt="690442830-844d33f4-1a2a-4a0c-81c9-efaa7261edc9" src="https://github.com/user-attachments/assets/8f4c0dbc-bd99-4fa0-a80c-890ed6c7dc3d" />

# Comparing Files
cmp file1 file2
## OUTPUT
<img width="570" height="207" alt="690442830-844d33f4-1a2a-4a0c-81c9-efaa7261edc9" src="https://github.com/user-attachments/assets/00c056a6-9231-465a-93e5-2731ee670b8a" />
 
comm file1 file2
 ## OUTPUT
<img width="552" height="257" alt="690443852-1ab25edc-8206-4456-8664-bc2bd3970a05" src="https://github.com/user-attachments/assets/673c9463-841a-4af<img width="552" height="257" alt="690443852-1ab25edc-8206-4456-8664-bc2bd3970a05" src="https://github.com/user-attachments/assets/27ea4cc8-93bc-4cb5-bc87-65d6fc87b285" />
a-9931-346dc0722ecf" />

 
diff file1 file2
## OUTPUT
<img width="552" height="257" alt="690443852-1ab25edc-8206-4456-8664-bc2bd3970a05" src="https://github.com/user-attachments/assets/aa2ac204-6069-4165-8b9c-0556cb09af0e" />


#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```


cut -c1-3 file11
## OUTPUT

<img width="547" height="71" alt="690449974-e6dd4523-42a7-4c0a-9e69-f8ec5b662c5c" src="https://github.com/user-attachments/assets/bcf5ff60-88b1-4a88-a7dc-b2832c423900" />



cut -d "|" -f 1 file22
## OUTPUT
<img width="711" height="85" alt="690460654-653a111d-8819-4d55-ad0f-5df8feba7777" src="https://github.com/user-attachments/assets/41a73116-2075-486a-b82f-7ce748a35add" />


cut -d "|" -f 2 file22
## OUTPUT
<img width="711" height="85" alt="690460654-653a111d-8819-4d55-ad0f-5df8feba7777" src="https://github.com/user-attachments/assets/0503a815-31d6-479e-bb0b-13ba7887aa65" />


cat < newfile 
```
Hello world
hello world
^d
````
cat > newfile 
Hello world
hello world
 
grep Hello newfile 
## OUTPUT

<img width="662" height="41" alt="690473496-c033cdb9-e9b8-4850-982a-b34e773b8a9d" src="https://github.com/user-attachments/assets/55c9433e-7127-439e-8a06-b5cabbf16a46" />


grep hello newfile 
## OUTPUT

<img width="667" height="37" alt="690473756-c4e858c2-d261-436d-8f9a-aeec9b916e90" src="https://github.com/user-attachments/assets/2177a606-41cd-4e7a-9d30-e7e8562d10b8" />



grep -v hello newfile 
## OUTPUT

<img width="700" height="45" alt="690474071-c619afd3-2254-4f64-b818-dae540a05471" src="https://github.com/user-attachments/assets/2c0a7de2-d547-4f4a-a219-4e971197a651" />


cat newfile | grep -i "hello"
## OUTPUT

<img width="808" height="67" alt="690474533-26efc89d-9abb-4405-9a0a-b60f00e06f29" src="https://github.com/user-attachments/assets/ddd9d205-da9f-4a77-93e6-8f8fa6652641" />



cat newfile | grep -i -c "hello"
## OUTPUT

<img width="842" height="45" alt="690474774-701cb1cf-ce8b-401e-b4ab-0ca330dcb99d" src="https://github.com/user-attachments/assets/b76f0a48-ad82-480c-8dbe-c2bbf22ad9f7" />



grep -R ubuntu /etc
## OUTPUT



grep -w -n world newfile   
## OUTPUT


cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```
egrep -w 'Hello|hello' newfile 
## OUTPUT

<img width="808" height="65" alt="690469911-d3070e23-6f30-452c-b226-681d45fed0f6" src="https://github.com/user-attachments/assets/ddfa2c59-12b3-4031-9c31-4dde508d8958" />


egrep -w '(H|h)ello' newfile 
## OUTPUT
<img width="776" height="65" alt="690470081-6ffd97e6-5dc0-4c64-a79b-319f55ba1f4e" src="https://github.com/user-attachments/assets/606f8d38-a2ec-467d-a10a-c7982ef6d092" />



egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT
<img width="828" height="65" alt="690470384-135c0cdd-9e8c-41a2-82eb-f1e23deb0fd6" src="https://github.com/user-attachments/assets/f2bcd580-3fe0-4049-81b5-d0991693394f" />





egrep '(^hello)' newfile 
## OUTPUT


<img width="733" height="42" alt="690470664-7e8b5b65-3285-4642-8ce3-1263e52fa040" src="https://github.com/user-attachments/assets/4c5f7fb0-22ed-4f93-b5ac-bc16d57e8178" />


egrep '(world$)' newfile 
## OUTPUT
<img width="745" height="67" alt="690470923-853d4fce-b05f-42da-a9fe-3aa4850ee2ae" src="https://github.com/user-attachments/assets/70a3895c-e532-4e81-beaf-bffb7dda5e70" />




egrep '(World$)' newfile 
## OUTPUT
<img width="745" height="67" alt="690470923-853d4fce-b05f-42da-a9fe-3aa4850ee2ae" src="https://github.com/user-attachments/assets/5dec0a34-3f2d-4553-8916-6840b08923d7" />


egrep '((W|w)orld$)' newfile 
## OUTPUT
<img width="782" height="66" alt="690471460-68cad66c-a8c8-4176-b660-30d33eed56a2" src="https://github.com/user-attachments/assets/45c7f474-a62d-42da-ba44-303ef25b6add" />



egrep '[1-9]' newfile 
## OUTPUT

<img width="701" height="43" alt="690471832-f7a866b8-8c0c-44b0-8f35-6aefc68f347c" src="https://github.com/user-attachments/assets/8feee67b-530a-41cf-b474-63e6bcebb9f0" />


egrep 'Linux.*world' newfile 
## OUTPUT
<img width="777" height="42" alt="690472153-69e873d8-e9a3-4d60-b83b-145b9cfed3df" src="https://github.com/user-attachments/assets/0ccca587-3803-4b0e-b2bd-7b7674b36422" />


egrep 'Linux.*World' newfile 
## OUTPUT
<img width="785" height="45" alt="690472287-ab4f22eb-b5f2-4c2c-903a-a22c6a138cba" src="https://github.com/user-attachments/assets/84c5bf32-df3b-43fa-9180-6feac3cb003e" />


egrep l{2} newfile
## OUTPUT

<img width="661" height="65" alt="690472486-0f1eda6c-5083-4a57-972f-0970937192fa" src="https://github.com/user-attachments/assets/19758873-6568-4ebe-b790-f3fe3ec226e5" />


egrep 's{1,2}' newfile
## OUTPUT 
<img width="711" height="87" alt="690472705-4e2437b7-490c-4fe9-a1aa-cdd6f80426ad" src="https://github.com/user-attachments/assets/24013d58-6bc5-4d19-997b-609220d4455a" />


cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```


sed -n -e '3p' file23
## OUTPUT
<img width="700" height="47" alt="690476543-924b6118-a0fc-40c3-bc71-60369b73150b" src="https://github.com/user-attachments/assets/9bb50865-56b5-49bd-9453-0f280ded6a87" />



sed -n -e '$p' file23
## OUTPUT
<img width="697" height="50" alt="690476831-3cd03458-0bbc-4935-92e1-19160615ae79" src="https://github.com/user-attachments/assets/54ee336a-9b98-4563-994f-e01c116c5ba4" />



sed  -e 's/Ram/Sita/' file23
## OUTPUT
<img width="780" height="205" alt="690478277-7ef66a32-da4e-45f7-9ef5-0ede968f024d" src="https://github.com/user-attachments/assets/7ab6742c-213d-4c4c-9bf5-dabe6913ba2e" />



sed  -e '2s/Ram/Sita/' file23
## OUTPUT
<img width="780" height="212" alt="690478652-d6dd1669-c6f6-4e90-ac91-f793eaa9033a" src="https://github.com/user-attachments/assets/ed6115f9-598e-456f-ae49-7339d3d7bbc5" />



sed  '/tom/s/5000/6000/' file23
## OUTPUT
<img width="806" height="207" alt="690478986-04f97e83-fec9-4acc-b07a-a8d4ab969f11" src="https://github.com/user-attachments/assets/f9408d51-d477-48ae-9b6b-5a70c664c809" />



sed -n -e '1,5p' file23
## OUTPUT
<img width="717" height="137" alt="690477608-c36eb84a-276a-482c-aee3-dd4979ddc934" src="https://github.com/user-attachments/assets/347fe111-ca20-46c8-830f-7f48b459c638" />



sed -n -e '2,/Joe/p' file23
## OUTPUT
<img width="770" height="90" alt="690479453-3e33513d-9fc0-42d4-a1ea-3b45617bd6e6" src="https://github.com/user-attachments/assets/d919c522-988c-44af-9ebd-88690480c504" />




sed -n -e '/tom/,/Joe/p' file23
## OUTPUT
<img width="817" height="67" alt="690479851-47213c6c-1330-4477-a9c5-66efd46acf2b" src="https://github.com/user-attachments/assets/5ded2ce3-795f-4013-b96d-e09bbcb2ecaf" />



seq 10 
## OUTPUT
<img width="521" height="260" alt="690480638-f36ba71f-98ee-460c-9ee2-8e46cda6a948" src="https://github.com/user-attachments/assets/f60e00aa-e86e-4b4a-8d43-8fd72047b61e" />



seq 10 | sed -n '4,6p'
## OUTPUT
<img width="706" height="90" alt="690480963-09ab3642-a8d2-4670-9a69-08755f81c794" src="https://github.com/user-attachments/assets/d8b72161-e41d-444e-80d8-9cf23a0956cd" />



seq 10 | sed -n '2,~4p'
## OUTPUT
<img width="728" height="93" alt="690481400-9925fc94-5deb-4cbf-95ef-707e07867d25" src="https://github.com/user-attachments/assets/aeda9ff2-76af-48d9-97b3-11c833c7c482" />



seq 3 | sed '2a hello'
## OUTPUT
<img width="703" height="116" alt="690482009-bf7e45a4-d057-4e0e-ae2b-f8836d4edfaa" src="https://github.com/user-attachments/assets/d3800cc5-9e8f-4661-b1d7-24b11c4b11af" />



seq 2 | sed '2i hello'
## OUTPUT
<img width="707" height="90" alt="690482376-408599cb-a51a-4c2c-9b08-ed6a25d488e5" src="https://github.com/user-attachments/assets/d892fcd1-5d20-43d8-86ae-1ef44e3ce902" />


seq 10 | sed '2,9c hello'
## OUTPUT
<img width="742" height="93" alt="690482715-30db2968-8295-4f56-bdfd-4fd358e1c049" src="https://github.com/user-attachments/assets/f5e1be6c-9510-4f65-a207-7597f270e7bc" />


sed -n '2,4{s/^/$/;p}' file23
## OUTPUT
<img width="795" height="95" alt="690483090-403021e9-a0ae-4f34-a759-532df0fe677c" src="https://github.com/user-attachments/assets/3871a2f1-761c-4ae8-b0f2-9d7964bdba5c" />



sed -n '2,4{s/$/*/;p}' file23
<img width="793" height="86" alt="690483557-3453e741-4eb4-40e9-bd9e-518bfdef32fd" src="https://github.com/user-attachments/assets/1a76e1bc-702a-4bfd-9793-f732c0197405" />


#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21
## OUTPUT
<img width="575" height="137" alt="690484830-55c45b2e-1cab-4a2e-bfd4-a8a52344978a" src="https://github.com/user-attachments/assets/46914851-78a4-4dfb-97c7-d74d6ff69823" />


cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22
## OUTPUT
<img width="585" height="137" alt="690485500-320144d0-22b0-4619-ac24-d196c42a0deb" src="https://github.com/user-attachments/assets/5565f8ac-2687-47f8-b3f0-dce07b2bfdff" />



#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT
<img width="872" height="207" alt="690485942-df0c51ad-8fb5-4f0a-bef1-b7eee9b9758e" src="https://github.com/user-attachments/assets/dab1d273-f7d7-4ff6-90ff-d0f7e3a6b114" />

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
cat urllist.txt | tr -d ' '
 ## OUTPUT
<img width="768" height="91" alt="690486783-ded148ab-bacd-49d2-aaaa-35a29fb5bf6f" src="https://github.com/user-attachments/assets/3ac7c39d-2263-43e2-9b21-b775eb2ea636" />


 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT
<img width="916" height="87" alt="690487424-75a64ed4-40de-4796-87be-a00d465ec823" src="https://github.com/user-attachments/assets/2459b9da-bb60-4d69-8d22-875470869926" />



#Backup commands
tar -cvf backup.tar *
## OUTPUT
<img width="708" height="205" alt="690488223-08206e00-745f-46c7-a597-1bcd53afb4f3" src="https://github.com/user-attachments/assets/8efc64f2-d2a0-4784-a917-a6ce18fa8d2d" />


mkdir backupdir
 
mv backup.tar backupdir

cd backupdir
 
tar -tvf backup.tar
## OUTPUT
<img width="810" height="212" alt="690489092-1c33658a-c00d-43f6-9392-5209c0675d3c" src="https://github.com/user-attachments/assets/ea22bdcc-4617-4c6b-b665-e13a7e256730" />


tar -xvf backup.tar
## OUTPUT
<img width="810" height="212" alt="690489092-1c33658a-c00d-43f6-9392-5209c0675d3c" src="https://github.com/user-attachments/assets/04334974-bc15-4f7f-a145-714ed5b7a9be" />


gzip backup.tar
<img width="803" height="210" alt="690489437-d1f4bf1f-44f5-4113-bdbb-97bb6afa9104" src="https://github.com/user-attachments/assets/630e7638-b36f-4679-bb8f-91cad15303d6" />

ls .gz
## OUTPUT
 <img width="803" height="210" alt="690489437-d1f4bf1f-44f5-4113-bdbb-97bb6afa9104" src="https://github.com/user-attachments/assets/af83c29b-988a-4cc4-b00d-e1edb47a11b0" />

 <img width="651" height="50" alt="690489930-75453f70-47ca-4fa5-8ca6-044e49a455c1" src="https://github.com/user-attachments/assets/7e9dffdc-2499-4935-bc87-c6fa51737c51" />
gunzip backup.tar.gz
## OUTPUT
<img width="651" height="50" alt="690489930-75453f70-47ca-4fa5-8ca6-044e49a455c1" src="https://github.com/user-attachments/assets/edbf9a51-32f2-4543-9b97-3e2b883ecd08" />

 # Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT
<img width="717" height="67" alt="690492636-12d0ba68-432f-4207-bfed-3785e5765267" src="https://github.com/user-attachments/assets/fe22e1fd-9947-4bdf-92da-cc1ff5d47c6f" />

<img width="903" height="131" alt="690491679-3338d1c5-4cd8-4afc-a164-6cf4dba965d3" src="https://github.com/user-attachments/assets/57387c03-a784-4f60-ab74-46867c7ed85f" />

 
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT
<img width="651" height="97" alt="690493408-fd4c538d-dc3d-42c1-94af-9a97854f16fb" src="https://github.com/user-attachments/assets/ab130537-d419-480c-a68a-fb2005d24dd3" />


cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT
<img width="711" height="342" alt="690494573-8511ec83-f5fc-4a0a-a137-795e95cd7fd5" src="https://github.com/user-attachments/assets/0448ebdf-79af-462b-ba41-f8b8bfe50d1c" />
ls file1
## OUTPUT
<img width="545" height="42" alt="690495825-172b1b7a-ae9e-40a2-928f-ca00c8974a59" src="https://github.com/user-attachments/assets/1c64ad61-b506-47c9-9ab7-f17156a0896b" />

echo $?
## OUTPUT 
<img width="526" height="42" alt="690496079-5c58b229-df44-4c13-a5ac-036e08e29103" src="https://github.com/user-attachments/assets/60eade0a-0bbb-47a2-a1eb-a3fae38660c4" />

./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
<img width="552" height="142" alt="690496613-24943441-9383-4963-b938-3a107a494e28" src="https://github.com/user-attachments/assets/f49db905-d112-4cd7-9499-20ff987707e4" />
 
abcd
 
echo $?
 ## OUTPUT
<img width="595" height="227" alt="690496943-b385c2c4-3bc0-495a-ba3f-9f44619d0083" src="https://github.com/user-attachments/assets/3e2ffca8-b536-4748-8ad4-850cf24691a6" />


 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
##OUTPUT
<img width="637" height="255" alt="690497830-6c0ddf33-d826-44bb-97ee-4a7de27ae543" src="https://github.com/user-attachments/assets/a2d2b3f8-1e8b-49d2-9950-ae18ae380daf" />




chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT
<img width="705" height="67" alt="690498049-63936cc2-51fa-4efc-b2a3-c19b5ab5a21a" src="https://github.com/user-attachments/assets/58a6a017-da58-485b-8ee1-5f2f37c9e8f1" />


# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT
<img width="655" height="47" alt="690499406-6ef740cf-46b7-4f43-9b7e-87619b84aa51" src="https://github.com/user-attachments/assets/2b254623-a8ef-4a2d-942a-2ad9b57b6a78" />

# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT
<img width="697" height="143" alt="690500996-266c437a-6af3-47d4-941c-cf2d468400c2" src="https://github.com/user-attachments/assets/f8f7c7f4-351a-4f40-ab2a-8d31e7ce282f" />



# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
##OUTPUT
<img width="662" height="122" alt="690501916-312bae67-4321-4ab8-a725-ef127c653e64" src="https://github.com/user-attachments/assets/b266f236-7240-4dca-84b3-1e004625f3d4" />


# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
##OUTPUT
<img width="710" height="116" alt="690502873-2e3b35c0-9031-4d90-b723-2ceb4a88e2ce" src="https://github.com/user-attachments/assets/85289959-6f0f-446b-a324-2b1eafa0de77" />

# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```
$ chmod 755 elifcheck.sh
 $ ./elifcheck.sh 

# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 
 
cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
 
 
cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
 
 
 
cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
 
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 
 
cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 
 
cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh

## OUTPUT
cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT


cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT
cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT
cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
## OUTPUT
$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT
cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT
$ ./exread1.sh 
 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT
 ./funcex.sh 

 
 ./funcex.sh 1 2

 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
 
 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 
cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT
 ./argshift.sh 1 2 3
 
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 
 
cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
# RESULT:
The Commands are executed successfully.
