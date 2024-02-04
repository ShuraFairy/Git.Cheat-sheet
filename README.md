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

������� --amend ������ � ���������� ������ ���������, ������� ������������ � �������. 
������������ � ��� �������������� ����������� commit message, ���� � ��� �������� ������.

git commit -m '��������� �������' -m '����� ��� ���������� �������'  # ������� ������ � ���������� � ���. �������

git commit <path> -m '���������'  # ����������� ��������� �������

git commit --amend [-m] # ����������� ��������� � ���������� ������
git commit --amend  --no-edit # ����������� ��������� � ���������� ������ ��� �������������� ��������� � ��������

```

## git push 
```shell
git push -u origin

���� -u (������ ������� --set-upstream) ������ � �������� ����������� �����, ��������������� ��������� � ��������� ��.

git push

������: git push -u origin master

��� ������� ������������ ��� �������� ������������� ������ � ��������� ����������� (����� ��������� ��� GitHub) � ��������� �����. 
����������� ��� �������, ����� �� ������� ����������� ����� � ��������� �����������. �� ����������� �����, ���� �� ����������� ��� �����. 
� � ��������� ��� ����� ����� ������������ ������� git push.

git push <remote> <branch>  # ��������� ��������� ����� �� remote 
git push -f <remote> <branch>  # ��������� ������������� ��������� ����� �� remote, ����������� � 
git push -u <remote> <branch>  # ���������� ��������� ����� �� remote � ������������� ������������
```

## git fetch
```shell
��� ������� ������������ ��� ��������� ����� ��������� ������ ������ ���������� �����������. 
��������� �������, ����� � ������ �� ���������� ����������� � ��� ��������� �����������.

git fetch # ��������� ��� ��������� �� origin 
git fetch <remote> # ��������� ��� ��������� �� remote
git fetch <remote> --prune # ��������� ��� ��������� �� remote � ���������������� ��
```

## git pull 
```shell
��� ������� ������������ ��� ���������� ������ ��� ���������� ���������� � �� �������� � ��������� �����������. 
git pull ��������� ����������� ���������� ���������� �����������.

git pull origin <branch>  # ������� �� remote ���������� ����� <branch> (�� ��������� ����� merge)
git pull origin <branch> --rebase  # ������� �� remote ���������� ����� � ������ rebase
```

## git branch 
```shell
��� ������� ������������ ��� ��������, ��������� �������������� � �������� �����, �� ������� �� ������ ����������. 

git branch -a # ������������ ��� ���������������� ��������� ���� ����� � ��������� �����������.
git branch -r # ������������ ��� ���������������� ��������� ���� ����� �� �������.
```

## git checkout \| switch
```shell
������: git checkout master ��� git checkout develop

��� ������� ������������ ��� ������������ �� �����, ������� �� ��� �������� �����.

git checkout � ��� ����  ������� �������������

git checkout <branch> | <commit>  # ������������� �� ����� ��� ������ �� ��� ����
git checkout -b <new_branch>  # �������������� �� ������� ����� � ����� ����� � ����� ������������� �� ��� �� ����� �����������

git switch <branch> | <commit> # ������������� �� ����� ��� ������ �� ��� ����
git switch -c <new_branch>  # �������������� �� ������� ����� � ����� ����� � ����� ������������� �� ��� �� ����� �����������
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

git merge <branch>  # ����� ��������� �� ����� <branch> � ������� �����
git merge --continue  # ���������� ������� � ������ ������� ����������
git merge --abort  # �������� merge
```

## git reset
```shell
git reset --hard HEAD

��� ������� ������ ��� ���������, ��������� ���� � ��� ��������� �����������, � ������� ��� �� ��������� 
������, ������� ���� ����������� �� GitHub.

git reset HEAD^

��� ������� ���������� ������� ����� ����� �� ��� �������, ���������� ������ ��� ��������, ������� �� 
������ ��� �������, �� ������� �������. �� �������� ��������� �������������� � ��������� ���������.

git reset <commit>  # �������� ������� � ������ �� ���������� �������
--soft  # ��������� ������������ � ������ (��������� ��������)
--hard  # ��������� ���������
git reset --soft HEAD~  # �������� ��������� ������ � ������
git reset --hard HEAD~4  # ����� ��������� 4 �������

# squash life-hack
git reset --soft HEAD~3  # ���������� 3 ��������� ������� � 1
git commit -m '���������� 3 �������'  # �������� ������, ��� ����� ��������� 3 ������� � 1
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

git rebase <commit>  # ������ ��������� ������� ����� �� ��������� ������ 
git rebase <branch>  # ������ ��������� ������� ����� �� ��������� �����
git rebase --continue  # ���������� ������� � ������ ������� ����������
git rebase --abort  # �������� rebase
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

## git log
```shell
git log  # ���������� ���� �� �������
git log <branch-name>  # ���������� ���� �� ���������� �����
git log --grep <pattern>  # ����� �������� � ���������� ����������
git log --invert-grep <pattern>  # ����� ��������, �� �������� � ���������
git log --oneline  # ������ �����, ������ � ����� ������
```

## git revert
```shell
git revert <commit>  # �������� ������
git revert -n <commit>  # �������� ������ � �������� ��������� � �������
```

## git reflog
```shell
git reflog  # �������� �������
git reflog <branch> # �������� ������� �� ���������� �����
```
