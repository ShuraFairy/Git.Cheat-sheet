# ������� Git, ������� ������ ����� ������ �����������

����� ���� ��������� ������-���������,  ������� �������� � ���� ������� �������, �� �� ���� �������� ������� Git, 
������� ����� ����� ������ ����������� ���������� � ����������.

## 0. help

git \<command\> --help  # ������� ���������� �� ������������� �������

git commit --help  # ������

## 1. git init

��� ������� ������������ ��� ������������� ������� ��� ����������� git.

git init \<name\>  # ������� ����������� � ������� ���������� � ������ \<name\>

## 2. git clone

��� ������� ��������� ����������� � ����� ����������. 

git config � ��� ������� �������, ������� ������������ ��� ��������� �������� ������������ Git �� ���������� � ��������� ������� �������. ������� ������:

git config --local user.name "Name"

git config --local user.email "your_email@example.com"

 git config --global user.name "Name"

 git config --global user.email "your_email@example.com"


���� ���� ����������� ������ �����:

git clone --depth=1 git://someserver/somerepo dirformynewrepo

rm -rf !$/.git 

## 3. git remote add

������: git remote add origin https://github.com/MrKrishnaAgarwal/Git-CheatSheet.git

��� ������� ������������ ��� ���������� ��� ����������� � ���������� �����������.

## 4. git remote -v

��� ������� ������������ ��� ��������� ������������ ��������� ������������.

## 5. git status

��� ������� ������������ ��� ��������� ������� ������ � ����� ��������� �����������. 
������������� �� �����? �� �������������? �������� �� ���?

## 6. git add

������: git add index.html

git add index.html style.css style.scss

��� ������� ��������� ��� ����� � ���������� ����� � ������ ������������������ ������

git add -A

��� ������� ������������ ��� �������������� ���� ��������������� ������.

git add

��� ����������� �����

�������� ��������� �� ����� ����������, ��������� ��� ������� �������
git add :/

���� ������������ �������� ����������
git add :/path/to/files/

�������� ������ � ������� ����������
cd test
git add .
������������ �����:
git add :/test

���� ������������ ������� ����������
cd test
git add ./path
������������ �����:
git add :/test/path


## 7. git reset

��� ������� ������������ ��� ������ ��� ������ ������ ���������, ��������� �������� ��������� ������� �� ������� �������. ��������. 

������ ��������������� �������: git reset --hard HEAD^

������ ������������� ������� ( ������� � ��������� ������� 7880ae2 )

git reset --hard f7880ae2

git push origin -f


## 8. git commit

��� ������� ��������� ������  � ����������� ������������� ����������.

git commit -m �Text message�

������: git commit -m "added navigation bar"

������� -m ��������� ������� commit message ��� ��������� � ���������

git commit --amend

������� --amend ������ � ���������� ������ ���������, ������� ������������ � �������. ������������ � ��� �������������� ����������� commit message, ���� � ��� �������� ������.


## 9. git push -u origin

���� -u (������ ������� --set-upstream) ������ � �������� ����������� �����, ��������������� ��������� � ��������� ��.

git push

������: git push -u origin master

��� ������� ������������ ��� �������� ������������� ������ � ��������� ����������� (����� ��������� ��� GitHub) � ��������� �����. 
����������� ��� �������, ����� �� ������� ����������� ����� � ��������� �����������. �� ����������� �����, ���� �� ����������� ��� �����. 
� � ��������� ��� ����� ����� ������������ ������� git push.

## 10. git fetch

��� ������� ������������ ��� ��������� ����� ��������� ������ ������ ���������� �����������. 
��������� �������, ����� � ������ �� ���������� ����������� � ��� ��������� �����������.

## 11. git pull 

��� ������� ������������ ��� ���������� ������ ��� ���������� ���������� � �� �������� � ��������� �����������. 
git pull ��������� ����������� ���������� ���������� �����������.

## 12. git branch ��� ������� ������������ ��� ��������, ��������� �������������� � �������� �����, �� ������� �� ������ ����������. 

git branch -a

��� ������� ������������ ��� ���������������� ��������� ���� ����� � ��������� �����������.

git branch -r

��� ������� ������������ ��� ���������������� ��������� ���� ����� �� �������.

## 13. git checkout

������: git checkout master ��� git checkout develop

��� ������� ������������ ��� ������������ �� �����, ������� �� ��� �������� �����.

git checkout � ��� ����  ������� �������������         

## 14. git merge

��� ������� ������������ ��� ����������� ���� �����. ��� ����� ������� �����, ������� �� ������ ������������ 
���������. � ��� �����, ������� �� ������ ������������ ������ � ���� ��������, � ��� �����, ������� ����������� ���������.

������: git merge develop

����� �������� ����� ��������� ��� �� ����� ����������.

## 15. git merge � abort

��� ������� ������������ ��� ������ �������.

���� ��� ������, ������� ����� ���������. �������������, ��� ���������� ����� ������������ ������ � ���������, 
����� ������� �� �������. ��� ������, ��� ����� ������������ ��� �������? ��� �������� ������, ��� ������� �� 
�������. �� ����� ����� ���������� ��� ��������� ��������� �������.

��� ��� ���� �������: ~/NextCloud/Documents/Web Projects/Cloud4Y (master)

���������� � ����� ����� ������. � ������� �������� (master). ��� ������, ��� �� ��������� � �������� �����. 
���� �� ���������� � ����� ����������, ��� ����� �������� (develop). ���� ��������� �� ����������, �������� 
������� (master|merging) ��� ���-�� � ���� ����. 

git merge -X theirs

������: git merge -X theirs develop

��� ������� ������������ ��� ����������� ���� �����. � ���� ���� ��������� �������, ��� ������� ������ 
�����������, ��� �� ������������� ���������, ��������� � ��������� ����� (� �� � �������).

# 16. git reset � hard HEAD

��� ������� ������ ��� ���������, ��������� ���� � ��� ��������� �����������, � ������� ��� �� ��������� 
������, ������� ���� ����������� �� GitHub.

# 17. git reset HEAD^

��� ������� ���������� ������� ����� ����� �� ��� �������, ���������� ������ ��� ��������, ������� �� 
������ ��� �������, �� ������� �������. �� �������� ��������� �������������� � ��������� ���������.

## 18. git clean -f

��� ������� ������������ ��� �������� ��������������� ������ ��  ������ ���������� �����������.

git clean -d

��� ������� ������������ ��� �������� ��������������� ���������� � ����� ��������� �����������. 
�� ����� ������ ���������� ��� � git clean -fd, ����� ������� � ��, � ������.

## 19. git rm -r � cached

������: git rm -r --cached config.js

��� ������� ������������ ��� �������� ����� �� ���������� ����������� (GitHub), �� ������ ��� � ��������� �����������.

## 20. git bisect

��� ������� ������������ ��� ����������� �������, ���������� ������ � ����. ��� ����� ��������� ������, 
��� ��� �������� � ������� ���������� ������.

## 21. git diff

git diff � ������ ������������� 

��� ������� ������������ ��������� ���������.

## 22. git rebase

�������, ���� �� �������� � ������, �� ����� ��� ����� ���������� ���������, ��������� � ���� �����, � ������. 
� ������� git rebase �� ������ ������������� ���� ����� ������ ��������� ������. ��� ����� �������, ���� ������� 
������� ������������ ����������� � ��������, ����� ��� ����������� �������� ������ ��� ���������� ��������� 
�������� �� ��������. ��� ������������ � �������� ��� �������������� ����� ��������.

git rebase -i HEAD~N

������� �������, ��������� ������� � ������� HEAD~N, �.�. � ����, ��� ���� N �������� �����. -i � �������� � ������������� ������.

## 23. git stash

��� ������� ������������ ��� ���������� ��������������� ��������� � ��������� ���������, ����� ����� ���� ��������� � ��� �����. ����  ����� ������������ � ��������� ���������. ������� �������, ����� �� ��������� ��� ����� ������, ������ ������������� �� ������, �� �� ��� �� ������ ������� ������ � ������� �����. ����� �������, �� ������� ��������� � ����, �������������� �� ������ �����, ������������� � �������� �����, � ����� �������������� ���� ���������.

git stash pop ��������� ��������� ����� ���������� ���������.

