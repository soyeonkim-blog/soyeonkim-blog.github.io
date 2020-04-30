---
---

# Learnig Github

<April 29, 2020>  
   
처음 Github 홈페이지를 만들었는데 시간이 생각보다 오래 걸렸다. 시간이 지나면 다시 만드는데 오래 걸릴 것 같으니, 메모해두기로 하자.   
지금 작성하고 있는 Github Markdown 문법에 4가지:   
- 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸 띄어쓰기 
- \<br/\>를 써줌으로써, 공백인 줄을 만들 수 있다.   
- 코드 표현을 위해서 으로 코드 앞뒤를 감싸기   
- {-}는 Markdown에서 bulleted list를 만들 수 있는 dot이 된다.  
   
<br/>
```
1. github로 repository 만들기   
{username}.github.io 로 repository name을 만들면, {username}.github.io 이 주소로 바로 연동이 가능해진다.   
   
   
   
   
2. 홈페이지 테마는 http://jekyllthemes.org/ 에서 고른다. 나는 'panthera-jekyll' 테마를 골랐다.   
git source code 다운   
   
$git clone https://github.com/christianezeani/panthera-jekyll.git   
   
   
   
   
3. 원도우10-ubuntu에서 내 로컬 폴더 디렉토리로 이동   
   
$cd /mnt/c/Users/soyeo/Desktop/panthera-jekyll-master/panthera-jekyll-master   
   
git 설치 및 version 확인
$git --version
# git version 2.17.1
   
$git config --global user.name soyeonkim-blog   
$git config --global user.email soyeon2019@gmail.com
   
$git init   
# Initialized empty Git repository in /mnt/c/Users/soyeo/Desktop/panthera-jekyll-master/panthera-jekyll-master/.git/

$git add . # 해당 디렉토리의 모든 파일을 add하는 코드. committed 되었다는 출력이 뜬다.   
$git commit -m "initial commit"
# [master (root-commit) c12c31b] initial commit
#
# 301 files changed, 75128 insertions(+)
# create mode 100644 .github/ISSUE_TEMPLATE/bug_report.md
# create mode 100644 .github/ISSUE_TEMPLATE/feature_request.md
# create mode 100644 .gitignore
# create mode 100644 Gemfile
# create mode 100644 LICENSE.txt
# create mode 100644 README.md

#git push -u origin master




4. local의 파일을 내 github repository에 push하는 경우, 서로 파일이 맞지 않아(?) 충돌로 인한 에러가 발생할 수 있다. 

$git remote add origin https://github.com/soyeonkim-blog/soyeonkim-blog.github.io.git
# fatal error 발생!

local파일을 강제로라도 repository에 push하고 싶은 경우, "git push -u origin +master"를 추가하여 임시로 해결할 수 있다.

$git push -u origin +master

#Username for 'https://github.com': soyeonkim-blog
#Password for 'https://soyeonkim-blog@github.com':
#Counting objects: 324, done.
#Delta compression using up to 4 threads.
#Compressing objects: 100% (315/315), done.
#Writing objects: 100% (324/324), 3.37 MiB | 984.00 KiB/s, done.
#Total 324 (delta 119), reused 0 (delta 0)
#remote: Resolving deltas: 100% (119/119), done.
#To https://github.com/soyeonkim-blog/soyeonkim-blog.github.io.git
# + 48b8c88...c12c31b master -> master (forced update)
#Branch 'master' set up to track remote branch 'master' from 'origin'.

web상에서 확인해보면, 폴더들과 파일들이 잘 upload되었음을 알 수 있다. 

```
