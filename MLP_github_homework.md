### `Git & Github ์ค๋ฌด ํ์ฉ`

***

#### ๐ป [Github ๊ณผ์  ๋งํฌ](https://github.com/han-gaeul/hello)



#### ๐ป Code

```python
# ์ ์ฅ์ ์์ฑ
git init

# ์๊ฒฉ ์ ์ฅ์ ์ฐ๊ฒฐ
git remote add origin https://github.com/han-gaeul/hello.git
  
# ๋ธ๋์น master์ 'hello.txt' ํ์ผ ์์ฑ
(master) touch hello.txt

# ํ์ผ ์์ฑ ์ปค๋ฐ
(master) git add .
(master) git commit -m 'create:hello.txt'

# ์๋ก์ด ๋ธ๋์น ์์ฑ
(master) git branch feature

# ๋ธ๋์น master์์ 'hello.txt' ํ์ผ ์์  ํ ์ปค๋ฐ
(master) git add .
(master) git commit -m 'edit:hello.txt'

# ๋ธ๋์น ์ด๋
(feature) git checkout feature

# ๋ธ๋์น feature์์ 'hello.txt' ํ์ผ ์์  ํ ์ปค๋ฐ
(feature) git add .
(feature) git commit -m '[feature] edit:hello.txt'

# ๋ธ๋์น master์ rebase
(feature) git rebase master

# 'Current branch feature is up to date' ๋ฉ์์ง๊ฐ ๋์ด
# ๊ตฌ๊ธ๋ง์ผ๋ก ํด๊ฒฐ ๋ฐฉ๋ฒ ์ฐพ๋ ๋์ค ๊ฐ์ ๋ก rebase ํ๋ ๋ฐฉ๋ฒ์ ์ฐพ์
(feature) git rebase --forse-rebase master

# ๋ธ๋์น master์ ๋ธ๋์น feature ๋ณํฉ
(master) git checkout master
(master) git merge feature

# ์ปค๋ฐ ํ ์๊ฒฉ ์ ์ฅ์์ push
(master) git add .
(master) git commit -m 'merge'
(master) git push origin master
```

<img src="MLP_github_homework.assets/homework.png" alt="homework" style="zoom:50%;" />

