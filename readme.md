
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


