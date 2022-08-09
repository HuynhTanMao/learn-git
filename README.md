echo "# vuvuzela" >> README.md

git init  //phải cùng cấp thư mục

git add README.md

or git add . // add all file and folder in current folder

git status

git commit -m "add README file"

git remote add origin https://github.com/HuynhTanMao/vuvuzela.git

or git remote add origin git@github.com:HuynhTanMao/vuvuzela.git // use ssh key

git remote -v // kiem tra trang thai ket noi voi github neu ra dung dòng mình add ở phan git remote add origin la dung

git push // up load lên git online

git pull // download tu online ve local

git restore `<file>` // xoa thay doi gat nhat

git reset <file> // huy file o trang thai staging -> working directory

git branch // show tat cac cac branch, muc dich cua viec tao nhieu branch để viet them tinh nang moi ma khong thay doi cau truc ban dau

git checkout - b <branch> // vd: "git checkout -b trang-chu" => tao them branch "trang-chu", chuyen working directory sang branch "trang-chu"

git checkout master // chuyen working directory sang branch "master"

git merge trang-chu // chuyen nhung thay doi tu branch "trang-chu" sang branch "master"

git branch -d <<branch>> // vd git branch -D trang-chu: xóa branch "trang-chu" sau khi hoàn thành tính năng để làm sạch master

or git push origin --delete <<branch>> vd git push origin --delete main: xóa branch "main" trên trang github.com (delete branch remotely)

git reset --soft <id-commit> //chuyen file tu trang thái commit sang trạng thái stage area // lay id commit git log or gitk, vd: git reset --soft

git reset --mixed <id-commit> //chuyen file tu trang thái commit sang trạng thái working directory // lay id commit git log or gitk, vd: git reset --soft

git reset --hard <id-commit> // chuyen file tu trang thai commit sang xóa hẳn file
