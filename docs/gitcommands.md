# BASIC GIT CONFIGURTION FOR BEGINNERS

To setup there are three levels of configuration

1. **--local** to set configuration for a single repo.
2. **--global** to set configuration for a your user.
3. **--system** to set configuration for all users.

Here i am using global in git configuration commmands, you can use any level of configuration as per your requirement.

Command to setup email:
  ```
  $git config --global user.email example@domain.com
  ```
  
Command to setup username:
  ```
  $git config --global user.name username
  ```
command to setup auto carriage return / line feed handling:
  ```
  $git config --global core.autocrlf true
  ```
command to setup default file editor:
```
  $git config --global core.editor vim 
```
command to setup certificate path:
```
  $git config --global http.sslCAInfo cacert.crt
```

command to skip ssl certification.

```
  $git config --global http.sslVerify false
```

command to setup credential help.

```
  $git config --global credential.helper 'cache --timeout=300'
```
  
Command to setup username and token:  

```
  $ git config --global github.user hemanth22
```

```
  $ git config --global github.token pastetokenhere
```

Command to setup default push configuration:
  ```
  $git config --global push.default simple
  ```
  *or*
  
  ```
  $git config --global push.default matching
  ```
  Difference between Simple and matching push.
  
  |**simple**|**matching**|
  |---|---|
|*Just Pushes current branch up to github.*|*Pushes all matching branches up to github.*|
  
Command to setup default pull configuration:
  ```
  $git config --global pull.rebase true
  ```
  By default **git pull** does *git fetch + git merge*
  If you feel useless merge appearing then you enable rebase using above command,
  or you can pull manually for any particular repo with rebase using below command line.
  ```$git pull --rebase``` this will perform *git fetch + git rebase*

  *In simple difference.*
  
  |**git with default pull**|**git with rebase pull**|
  |---|---|
  |$git pull|$git pull --rebase|
|<ul><li>$git fetch</li><li>$git merge</li></ul>|<ul><li>$git fetch</li><li>$git rebase</li></ul>|
     
Command to setup resue recorded resolution:
  ```
  $git config --global rerere.enabled true
  ```
  
Command to create aliases:  
  ```
  $git config --global alias.s "status -s"
  $git config --global alias.lg "log --oneline --decorate --all --graph"
  $git config --global alias.lg "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"
  ```
Command to setup by pass for longpaths.  
  ```
  $git config --system core.longpaths true
  ```
Command to setup colour ui:
  ```
  $git config --global color.ui true
  ```
command to list the setup:
  ```
  $git config --global --list
  ```
   *or*
  
  ```
  $cat ~/.gitconfig
  ```
Command to remove configuration for any section.
  ```
  $git config --global --remove-section [section-name]
  ```
  Example
  ```
  $git config --global --remove-section pull
  ```
  
Steps to configure to git completion.
```
$curl -0L https://github.com/git/git/raw/master/contrib/completion/git-completion.bash > git-completion.bash
```
```
$mv ~/git-completion.bash ~/.git-completion.bash
```

Add below configuration unix profile.
```                                                                                                  
               # .git_completion                                                         
               if [ -f ~/.git-completion.bash ]; then                            
                   source ~/.git-completion.bash                                 
                fi                                                                                 
 ```                           
 
 
