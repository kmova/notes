#Migrating to bitbucket
[Steps for migrating to BitBucket](https://www.atlassian.com/git/tutorials/migrating-overview)
## Prepare
```
mhost#ssh <ubuntu host>
mhost#mkdir bb_migration
mhost#cd bb_migration/
mhost#wget https://bitbucket.org/atlassian/svn-migration-scripts/downloads/svn-migration-scripts.jar .
mhost#java -jar svn-migration-scripts.jar verify
mhost#java -jar ~/svn-migration-scripts.jar authors <svn-repo> > authors.txt (If this is not compatible)
mhost#svn log svn+ssh://username@ipaddress/svnrepo/esports | grep line | awk '{print $3}' | sort | uniq | more | awk '{print $1," = ",$1, " <",$1"@cloudbyte.com>"}'
```
