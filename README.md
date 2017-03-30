# datascience

echo "# datasciencecoursera" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/cesarhsfranca/datasciencecoursera.git
git push -u origin master


# datascience

Dear colleagues,
first of all I would like to mention some dificulties I found while using the command "Push" as below described:


I could not understand why I received the below error message:


$ git push -u origin master
remote: Repository not found.

fatal: repository 'https://github.com/cesarhsfranca/datascience.git/' not found



The reason for that is because first I created the repository named "datasciencecoursera" and the "push" command was always trying to find 
the repository named "datascience" 
which was not originally created.

Only after I have created the repository named "datascience" it 
worked as expected.



The whole sequence that worked for me is as follow:


echo "# datasciencecoursera" >> HelloWorld.md

git init
git add Helloworld.md

git commit -m "first commit"

git remote add origin https://github.com/cesarhsfranca/datascience.git

git push -u origin master


The above commands produced the following results in Git:


Counting objects: 6, done.

Delta compression using up to 4 threads.

Compressing objects: 100% (3/3), done.

Writing objects: 100% (6/6), 590 bytes | 0 bytes/s, done.

Total 6 (delta 0), reused 0 (delta 0)

To https://github.com/cesarhsfranca/datascience.git
 * [new branch]  master -> master

Branch master set up to track remote branch master from origin.


