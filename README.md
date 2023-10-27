## Introduction

key:  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

Hãy bắt đầu bằng việc mở Git Bash và định cấu hình nó bằng tên người dùng và ID email.

Để cấu hình, chúng ta sử dụng lệnh sau:
##
Git config --global user.name "Simplilearn GitHub"
Git config --global user.email siddam.bharat@simplilearn.net
Git config –list
##

![image](https://github.com/bqminh30/git-demo/assets/64219602/c03bf776-4ed2-430a-bd45-e9d651feae95)

Sau đó, hãy kiểm tra thư mục làm việc hiện tại:
##
pwd
##

![image](https://github.com/bqminh30/git-demo/assets/64219602/00396eba-e3df-40f6-9b50-4913d183ebc5)

Để tạo một kho lưu trữ trong thư mục làm việc, hãy sử dụng các lệnh sau:
##
mkdir Git_Demo
cd Git_Demo
pwd
##
Chúng ta có thể đến vị trí thư mục và kiểm tra thư mục Git_demo.

![image](https://github.com/bqminh30/git-demo/assets/64219602/e48cc0bb-ffb5-44ec-94d3-b11b33ece8b9)

Thư mục "Git_demo" hiện tại sẽ trống.

Hãy tạo một thư mục cho kho lưu trữ.
##
mkdir FirstRepo
cd FirstRepo
pwd
##

![image](https://github.com/bqminh30/git-demo/assets/64219602/7011e3b8-9d0b-43d3-a199-77350ab03d78)

Thư mục "FirstRepo" trống. Bây giờ chúng ta sẽ khởi tạo một kho lưu trữ vào thư mục của mình.
##
Git init
##

![image](https://github.com/bqminh30/git-demo/assets/64219602/1e7609f9-efe0-4551-bd56-7b14a38b7e7d)

Thứ được gọi là "master" xuất hiện trên màn hình. Bất cứ khi nào kho lưu trữ Git được tạo lần đầu tiên, nó sẽ tạo một nhánh và tên của nhánh đó là master. Điều hướng đến thư mục; bạn có thể tìm thấy thư mục ".git" ẩn.

Nếu bạn kiểm tra thư mục, bạn có thể thấy một số thư mục và cấu hình. Đảm bảo bạn không thực hiện bất kỳ thay đổi nào đối với bất kỳ thư mục nào.

![image](https://github.com/bqminh30/git-demo/assets/64219602/a30dbe9f-44dd-4863-ad18-0207b85b6fc9)

Tạo hai file và ghi lại từng cái một.
Đối với notepad đầu tiên, các lệnh như sau:
##
touch alpha.txt
notepad alpha.txt
##

![image](https://github.com/bqminh30/git-demo/assets/64219602/77221d59-116e-4bea-8a8e-ddc20723643a)

Tiếp theo, hãy kiểm tra trạng thái của file đã được tạo.
git status

![image](https://github.com/bqminh30/git-demo/assets/64219602/3edeff63-b37e-4347-bfd4-5600194424af)

git add .

![image](https://github.com/bqminh30/git-demo/assets/64219602/fde2200a-474b-467b-a0ee-a71f89959b06)

git commit -m "alpha"

![image](https://github.com/bqminh30/git-demo/assets/64219602/4a635802-23ad-49e9-8c83-04e9cfdc6897)

Hãy kiểm tra lại trạng thái của file.

![image](https://github.com/bqminh30/git-demo/assets/64219602/11d21a3e-b524-415b-8a60-aeecdef52004)

Bây giờ, hãy đẩy hai notepad trên GitHub. Mở tài khoản GitHub của bạn và tạo một kho lưu trữ mới. Tên của kho lưu trữ sẽ là "FirstRepo."

![image](https://github.com/bqminh30/git-demo/assets/64219602/947fab64-c11f-4695-b8e4-31c29b4d6ded)

Sao chép URL "git remote add origin" URL.

![image](https://github.com/bqminh30/git-demo/assets/64219602/0bd232bd-a32b-4218-bc12-45bf14da8aa2)

Dán URL đã sao chép vào Git Bash.

![image](https://github.com/bqminh30/git-demo/assets/64219602/fab1ff30-451b-4f22-8697-d396b5cdcbaf)

##
git remote -v
##

![image](https://github.com/bqminh30/git-demo/assets/64219602/257477f5-e4ba-4e9c-a85c-2f2545e52e44)

Bây giờ, hãy push nội dung vào kho lưu trữ từ xa.
##
git push -u origin master
##

<img width="755" alt="Screen Shot 2023-10-13 at 22 17 53" src="https://github.com/bqminh30/git-demo/assets/64219602/addaac04-7d4b-4d51-9934-f202e4c7bdd0">

<img width="755" alt="Screen Shot 2023-10-13 at 22 18 58" src="https://github.com/bqminh30/git-demo/assets/64219602/934358ce-a4b8-4d26-a780-e5bf7f1d7831">

##1......<<<<<<< HEAD=======2......3......>>>>>>> dev_a4......
Có thể hiểu những dòng mới trong file person.java này là "Conflict deviders" bộ chia xung đột. Trong đó: 
+ Đầu tiên, dòng "<<<<<<< HEAD" là nội dung tồn tại trong nhánh master hiện tại mà tham chiếu HEAD đang trỏ tới.
+ Thứ hai, tất cả nội dung phía sau dòng "=======" là "trung tâm" của cuộc xung đột. Thể hiện nội dung xung đột. 
+ Thứ ba, tất cả nội dung phía sau dòng ">>>>>>> dev_a" là nội dung có trong nhánh dev_a chuẩn bị hợp nhất vào master.




