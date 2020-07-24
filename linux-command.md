# clean RAM
sudo purge

# cd
cd ~ (вернуться в домашнюю директорию)

# touch (создать файл)
touch file__name

# grep (найти)
grep "some string" file
grep -i "REact" file (case insensitive
grep -c "react" index.js (c is for count)

# cat
cat .bashrc | less (показать файл + использовать less, q - выйти)
cat somefile > somefile2 (copy and create from file somefile to somefile2)

# mkdir
mkdir some-directory

mkdir -p /foo/bar/baz  # creates bar and baz within bar under existing /foo

# rm
rm -rf some-directory

# rmdir
rmdir some-directory (removes empty directory)

# find
find path -name filename
find . -name "*.js"

# mv
mv somefile /to/some/other/path
mv ~/Documents/Ukulele/Apache.pdf . (from ~/Documents/Ukulele/Apache.pdf to current folder)

# alias
alias pf="ps -e | grep $1" (pf shutter - пример найти PID процесса shutter)

# kill
kill pid-of-program (ps -e | grep webstorm, затем kill PID)

# find and kill process on port
Find:
sudo lsof -i :3000
Kill:
kill -9 <PID>

# get all PATH
echo $PATH

# get username
whoami

# add permission to folder for user (have to open terminal inside folder)
sudo chown __use-name__ .

# add path to $PATH
export MONGO_PATH=/Users/max/mongodb
export PATH=$PATH:$MONGO_PATH/bin

or

export PATH=$PATH:~/mongodb/bin (inside user directory)

# mongo
(create folder for mongo to store its data)
mkdir -p /data/db 

(launch mongo)
sudo mongod

# echo
echo "export VAR_NAME='VAR_VALUE''" > var-file.env
echo "var-file" >> .gitignore
source ./var-file.env

# create gzip
cat ./dist{file1, file2, file3}.js | gzip > gulpfile.js.gzip - //собрать все в 1 файл и добавить в gzip
