<h1>Phần Test Conflict</h1>
Sau khi sửa 1 file b.html trên website và sửa bản clone tại máy local cùng 1 lúc

dữ liệu thông báo: 

![image](https://github.com/user-attachments/assets/f5fc3964-c5d6-4ea8-a6a6-e0713ba276f9)

dữ liệu hiển thị trên trình soạn thảo :

![image](https://github.com/user-attachments/assets/a5ae47a0-ee22-4406-bf0e-3b265052b275)

<h1>Phần ba trạng thái</h1>
Ba trạng thái bao gồm : Modified, Staged, Committed
sử dụng các lệnh như là :
<h3>Modified: </h3>
echo "new content" >> b.html
<h3>Staged: </h3>
git add b.html
<h3>Committed: </h3>
git commit -m "Update b.html with new content"  

<h3>Log của trạng thái thứ 3:</h3>
[release 5832b4e] Update b.html with new content
 1 file changed, 0 insertions(+), 0 deletions(-)

