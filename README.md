# probable-guide
My CLI CheatSheet
Git
Download the repo
git clone https://github.com/peter-yeh/ComputerOS.git

Get change from github, do it before making changes to get the latest update
git pull

Check status of current branch
git status

Stage all changes
git add .

Add All changes
git commit -m 'First commit'

Push all changes to github
git push

ssh
Move files from local storage to remote location, e.g. sunfire
scp lab1.tar.gz yuchun@sunfire.comp.nus.edu.sg:lab1.tar.gz

Move files from sunfire to xcne5, -r for whole folder recursive
scp lab1.tar.gz yuchun@xcne5:lab1.tar.gz

Comparing files/ testing labs
Compile the c code into exe format
gcc ex1.c -o ex1.exe

Compare the answers
./ex1.exe < test1.in

./ex1.exe < test1.in > myOut1.txt

diff test1.out myOut1.txt

Unzip the zip files
gunzip -c lab1.tar.gz | tar xvf -

Remove whole folder -r recusrive
yes | rm -r folder // for sunfire since it keeps asking confirmation

rm -r folder // for xcne

Checking files b4 submission
Zip files in the L1 folder
zip A0123456X.zip ex2/ex2.c ex3/ex3.c

Check if zip file structure is of the correct layout
chmod +x ./check_zip.sh

./check_zip.sh A0123456X.zip

