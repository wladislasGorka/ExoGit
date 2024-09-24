Exo Git  

modif branch-a  
modif branch-b  

Exercice GIT base manip  

1/ créer un dossier de projet  
	mkdir ExoGit  

2/ créer 3 dossiers (html/css/js)  
	mkdir html  
	mkdir js  
	mkdir css  

3/ créer les fichiers index.html, index.js et styles.css dans leurs dossiers respectifs  
	New-Item .\html\index.html  
	New-Item .\js\index.js  
	New-Item .\css\style.css  

4/ mettre a jour l'ensemble dans le dossier remote  
	Publish on Github  

5/ créer une branche "dev"  
	git checkout -b dev  
	git push -u origin dev  

6/ lister les branches  
	git branch  

7/ se positionner sur la branche dev  
	git switch dev  

8/ modifier le fichier css  

9/ mettre la modif a jour sur la branche dev  
	git commit -a -m "change css"  
	git push  

10/ revenir sur la branche master et ouvrir le fichier css (voit-on la modif ?)  
	Non.  

11/ fusionner la branche dev sur la branche master  
	git switch main  
	git merge --no-ff dev  

12/ verifier la modif css  

13/ retourner sur la branche dev et ajouter un fichier readme.md  
	git switch dev  
	New-Item .\readme.md  

14/ faire un commit de ce fichier  
	git add .\readme.md  
	git commit -a -m "add readme"  

15/ visualiser les differences avec la commande adéquate  
	git diff  

16/ créer deux nouvelles branches branch-a et branch-b  
	git checkout -b branch-a  
	git push -u origin branch-a  
	git checkout -b branch-b  
	git push -u origin branch-b  

17/  dans chaque fichier readme de chaque branche, ajoutez une ligne spécifique (modif branch-a et branch-b par ex)  

18/ comparez les deux branches avec la fonction adéquate  
	git diff branch-a branch-b  

19/ mergez la branche a sur master  
	git switch main  
	git merge --no-ff branch-a  

20/ mergez la branche b sur master  
	git merge --no-ff branch-b  

21/ essayez de resoudre le conflit ...  
	une fois que le merge est OK  
	git push  



