Examen mi-session-PARTIE3

# Partie 1 : Préparation du Dépôt GitHub

1.  Create directory jenkins-data-pipeline and initialize git.

```bash
vboxuser@ubuntu2204-Jenkings:~/Documents$ mkdir jenkins-data-pipeline
vboxuser@ubuntu2204-Jenkings:~/Documents$ cd jenkins-data-pipeline/
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ git init
Initialized empty Git repository in /home/vboxuser/Documents/jenkins-data-pipeline/.git/

```

2.  Create this current README.md file

```bash
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ git add .
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ git commit -m "add README file"
```

3.  Create in github jenkins-data-pipeline repository and clone in local jenkins-data-pipeline


```bash
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ git remote add origin https://github.com/cpelaezdc/jenkins-data-pipeline.git
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ git branch -M main
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ git push -u origin main
Username for 'https://github.com': cpelaezdc
Password for 'https://cpelaezdc@github.com':
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 268 bytes | 89.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/cpelaezdc/jenkins-data-pipeline.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
```

4.   Add others files to this project"

```bash
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ nano data_analysis.py
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ nano sales_data.csv
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        data_analysis.py
        sales_data.csv

nothing added to commit but untracked files present (use "git add" to track)
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ git add .
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ git commit -m "Initial commit with adv
anced data anlysis script"
vboxuser@ubuntu2204-Jenkings:~/Documents/jenkins-data-pipeline$ git push origin main
```


# Partie 2 : Configuration du Pipeline Jenkins

1.   Add a new job as pipeline

![alt text](image.png)

![alt text](image-2.png)

![alt text](image-3.png)

![alt text](image-4.png)



