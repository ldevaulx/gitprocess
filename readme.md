
# Creation d'une branche de feature

    git checkout develop
    git fetch origin
    git pull -rebase develop
    
    git checkout -b feature/some_feature

travailler sur la feature
pusher pour faire des sauvegardes régulières

    git push origin feature/some_feature


Rester à jour des évolutions de develop régulièrement

    git fetch origin
    git rebase origin/develop

## Passer en production

    git tag x.x.0
    git push origin x.x.0

    git checkout master
    git merge 1.0.0
    git push origin master

# Creation d'un patch

    git checkout x.x.0
    git checkout -b hotfix/x.x.1

## Passage en production

    git tag x.x.1
    git push origin x.x.1

    git checkout master
    git merge x.x.1
