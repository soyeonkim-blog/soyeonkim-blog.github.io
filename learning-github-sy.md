---
---

# Learnig Github

<April 29, 2020>  
   
처음 Github 홈페이지를 만들었는데 시간이 생각보다 오래 걸렸다. 시간이 지나면 다시 만드는데 오래 걸릴 것 같으니, 메모해두기로 하자.   
지금 작성하고 있는 마크다운 문법에 2가지:   
(1) 줄 바꿈을 하기 위해서는 문장 마지막에서 3칸 띄어쓰기   
(2) 코드 표현을 위해서 "```"으로 코드 앞뒤를 감싸기 
     
```
1. github로 repository 만들기   
{username}.github.io 로 repository name을 만들면, {username}.github.io 이 주소로 바로 연동이 가능해진다. 

2. http://jekyllthemes.org/

# 원도우10에서 제공하는 ubuntu에서 내 로컬에 다운 받아둔 지킬 테마 폴더 디렉토리로 이동 

cd /mnt/c/Users/soyeo/Desktop/panthera-jekyll-master/panthera-jekyll-master

# https://gist.github.com/godori/355391c91d2f6725aee8f273f095e87c

git --version
# git version 2.17.1

git config --global user.name soyeonkim-blog
git config --global user.email soyeon2019@gmail.com

git init
# Initialized empty Git repository in /mnt/c/Users/soyeo/Desktop/panthera-jekyll-master/panthera-jekyll-master/.git/

git add . # 모든 파일을 add하겠다. committed 되었다고 뜬다. 

git commit -m "initial commit"
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

git remote add origin https://github.com/soyeonkim-blog/soyeonkim-blog.github.io.git

git push -u origin +master # 강제 push 실제 에러가 발생하는 부분을 고칠수도 있지만 임시 방편으로 "+" 를 이용하여 해결이 가능합니다
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
```
