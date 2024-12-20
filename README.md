## Getting started

git clone https://gitlab.com/hundle1/deha-academy-dev-php-git-lab.git

<h1> WorkFlow of # Deha-Academy-Dev-php-git-Lab</h1>


## 1. Tạo projects:

![st1](https://github.com/user-attachments/assets/f2caf460-a639-45a9-9ca2-937e95ef8c33)


## 2. Tạo nhánh Develop
git checkout -b develop

git push -u origin develop

![st2](https://github.com/user-attachments/assets/1e42b8cb-a7a5-41f4-a680-f51b47d9ce73)

## 3. Tạo nhánh feature
git checkout -b feature/login_component develop
(from develop, khỏi pull)

git add index.html

git commit -m "Add login component"

git push -u origin feature/login_component

![st3](https://github.com/user-attachments/assets/686cce28-beaa-4542-bf30-7cc6fdd75ae2)

git checkout -b feature/logout_component develop

git add index.html

git commit -m "Add logout component"

git push -u origin feature/logout_component

![st4](https://github.com/user-attachments/assets/fa0f2930-767f-480d-8661-77f7ceb151d6)

## 4. Merge các nhánh feature vào develop
### 4.1 Merge bằng IDE:
git checkout develop

git merge feature/login_component

git push

git merge feature/logout_component

git push

![st5](https://github.com/user-attachments/assets/1b09e54a-c52c-4d0b-9558-73038291c266)

trong khi merge logout thì gặp CONFLICT và đã sửa 

![conflict](https://github.com/user-attachments/assets/070eeec5-76eb-4feb-9793-34c1ef55e484)

### 4.2 Merge bằng server gitlab:

![merge request on server](https://github.com/user-attachments/assets/445e00f3-a5ad-49c3-a64c-f4dda5b37c86)

## 5. Tạo nhánh release
git checkout -b release/v0.1 develop

git commit -am "Prepare release v0.1"

git push -u origin release/v0.1

![st6](https://github.com/user-attachments/assets/7cc5691d-e3ef-4cec-af5a-78675686fd9f)

## 6. Tạo và xử lý Hotfix 

git checkout -b hotfix/fix-login-bug develop 

Thêm 1 dòng vào file index.html ( đã thêm bên dưới login)

git commit -am "Fix login bug"

git push -u origin hotfix/fix-login-bug

![st7](https://github.com/user-attachments/assets/00e43cee-ca71-4501-bcb4-df1571e732e1)


## 7. Merge Hotfix vào main và develop

git checkout main

git merge hotfix/fix-login-bug

git push


git checkout develop

git merge hotfix/fix-login-bug

git push

<h1>License</h1>

Feel free to clone XD - Hundle1 psssss
