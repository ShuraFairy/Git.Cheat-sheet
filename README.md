# ������� Git, ������� ������ ����� ������ �����������

����� ���� ��������� ������-���������,  ������� �������� � ���� ������� �������, �� �� ���� �������� ������� Git, 
������� ����� ����� ������ ����������� ���������� � ����������.

## help
```shell
git <command> --help  # ������� ���������� �� ������������� �������
git commit --help  # ������
```

## git init
```shell
��� ������� ������������ ��� ������������� ������� ��� ����������� git.
git init <name>  # ������� ����������� � ������� ���������� � ������ \<name\>
```

## git clone
```shell
��� ������� ��������� ����������� � ����� ����������. 

git config � ��� ������� �������, ������� ������������ ��� ��������� �������� ������������ Git �� ���������� � 
��������� ������� �������. ������� ������:

git config --local user.name "Name"
git config --local user.email "your_email@example.com"
git config --global user.name "Name" 
git config --global user.email "your_email@example.com"

���� ���� ����������� ������ �����:
git clone --depth=1 git://someserver/somerepo dirformynewrepo
rm -rf !$/.git 
```

## git remote
```shell
git remote add

������: git remote add origin https://github.com/MrKrishnaAgarwal/Git-CheatSheet.git

��� ������� ������������ ��� ���������� ��� ����������� � ���������� �����������.

git remote set-url origin https://github.com/LpilinAlexandr/basic-git123.git  # �������� � origin remote �����
git remote add test https://github.com/LpilinAlexandr/basic-git123.git  # ���������� ����� remote �����       
git remote -v  # ���������� ������ ���� remote �������
```

## git status
```shell
��� ������� ������������ ��� ��������� ������� ������ � ����� ��������� �����������. 
������������� �� �����? �� �������������? �������� �� ���?

git status -s  # ������ � �������� �����
```

## git add \| restore \| rm
```shell
git add <path>  # �������� � ������ ��� ���������� ��� ���� �� ���������� ����
git add .  # �������� �� � ������� ����������

git restore --staged <path>  # ��������� �� ������� ����������� ���������� ��� ���� �� ���������� ����
git restore <path>  # �������� ��������� � ��������� ����� 

git rm  # ���������� �� �� �����, ��� � �������� �����/����������

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
```

## git reset
```shell
��� ������� ������������ ��� ������ ��� ������ ������ ���������, ��������� �������� ��������� ������� �� ������� �������. ��������. 

������ ��������������� �������: git reset --hard HEAD^

������ ������������� ������� ( ������� � ��������� ������� 7880ae2 )

git reset --hard f7880ae2

git push origin -f
```

## git commit
```shell
��� ������� ��������� ������  � ����������� ������������� ����������.

git commit -m �Text message�

������: git commit -m "added navigation bar"

������� -m ��������� ������� commit message ��� ��������� � ���������

git commit --amend

������� --amend ������ � ���������� ������ ���������, ������� ������������ � �������. ������������ � ��� �������������� ����������� commit message, ���� � ��� �������� ������.
```

## git push -u origin
```shell
���� -u (������ ������� --set-upstream) ������ � �������� ����������� �����, ��������������� ��������� � ��������� ��.

git push

������: git push -u origin master

��� ������� ������������ ��� �������� ������������� ������ � ��������� ����������� (����� ��������� ��� GitHub) � ��������� �����. 
����������� ��� �������, ����� �� ������� ����������� ����� � ��������� �����������. �� ����������� �����, ���� �� ����������� ��� �����. 
� � ��������� ��� ����� ����� ������������ ������� git push.
```

## git fetch
```shell
��� ������� ������������ ��� ��������� ����� ��������� ������ ������ ���������� �����������. 
��������� �������, ����� � ������ �� ���������� ����������� � ��� ��������� �����������.
```

## git pull 
```shell
��� ������� ������������ ��� ���������� ������ ��� ���������� ���������� � �� �������� � ��������� �����������. 
git pull ��������� ����������� ���������� ���������� �����������.
```

## git branch 
```shell
��� ������� ������������ ��� ��������, ��������� �������������� � �������� �����, �� ������� �� ������ ����������. 

git branch -a

��� ������� ������������ ��� ���������������� ��������� ���� ����� � ��������� �����������.

git branch -r

��� ������� ������������ ��� ���������������� ��������� ���� ����� �� �������.

## git checkout

������: git checkout master ��� git checkout develop

��� ������� ������������ ��� ������������ �� �����, ������� �� ��� �������� �����.

git checkout � ��� ����  ������� �������������
```

## git merge
```shell
��� ������� ������������ ��� ����������� ���� �����. ��� ����� ������� �����, ������� �� ������ ������������ 
���������. � ��� �����, ������� �� ������ ������������ ������ � ���� ��������, � ��� �����, ������� ����������� ���������.

������: git merge develop

����� �������� ����� ��������� ��� �� ����� ����������.

git merge � abort

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
```shell

## git reset
```shell
git reset --hard HEAD

��� ������� ������ ��� ���������, ��������� ���� � ��� ��������� �����������, � ������� ��� �� ��������� 
������, ������� ���� ����������� �� GitHub.

git reset HEAD^

��� ������� ���������� ������� ����� ����� �� ��� �������, ���������� ������ ��� ��������, ������� �� 
������ ��� �������, �� ������� �������. �� �������� ��������� �������������� � ��������� ���������.
```

## git clean -f
```shell
��� ������� ������������ ��� �������� ��������������� ������ ��  ������ ���������� �����������.

git clean -d

��� ������� ������������ ��� �������� ��������������� ���������� � ����� ��������� �����������. 
�� ����� ������ ���������� ��� � git clean -fd, ����� ������� � ��, � ������.
```

## git rm -r � cached
```shell
������: git rm -r --cached config.js

��� ������� ������������ ��� �������� ����� �� ���������� ����������� (GitHub), �� ������ ��� � ��������� �����������.
```

## git bisect
```shell
��� ������� ������������ ��� ����������� �������, ���������� ������ � ����. ��� ����� ��������� ������, 
��� ��� �������� � ������� ���������� ������.
```

## git diff
```shell
git diff � ������ ������������� 

��� ������� ������������ ��������� ���������.
```

## git rebase
```shell
�������, ���� �� �������� � ������, �� ����� ��� ����� ���������� ���������, ��������� � ���� �����, � ������. 
� ������� git rebase �� ������ ������������� ���� ����� ������ ��������� ������. ��� ����� �������, ���� ������� 
������� ������������ ����������� � ��������, ����� ��� ����������� �������� ������ ��� ���������� ��������� 
�������� �� ��������. ��� ������������ � �������� ��� �������������� ����� ��������.

git rebase -i HEAD~N

������� �������, ��������� ������� � ������� HEAD~N, �.�. � ����, ��� ���� N �������� �����. -i � �������� � ������������� ������.
```

## git stash
```shell
��� ������� ������������ ��� ���������� ��������������� ��������� � ��������� ���������, ����� ����� ���� ��������� 
� ��� �����. ����  ����� ������������ � ��������� ���������. ������� �������, ����� �� ��������� ��� ����� ������, 
������ ������������� �� ������, �� �� ��� �� ������ ������� ������ � ������� �����. ����� �������, �� ������� ��������� 
� ����, �������������� �� ������ �����, ������������� � �������� �����, � ����� �������������� ���� ���������.

git stash pop # ��������� ��������� ����� ���������� ���������.

git stash -m 'my stash name'  # ������� ��� ��������� � ���� 

git stash pop  # �������� ��������� ��������� �� �����, ������ ��� ������. �� ������� 0

git stash apply  # �������� ��������� ��������� �� �����, �������� ���. �� ������� 0

git stash list  # ���������� ������ ���� ������

git stash show <stash>  # ���������� ����. �� ������� 0

git stash drop <stash>  # ������� ����. �� ������� 0
```
