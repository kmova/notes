## Configure Passwordless SSH between two nodes with the same username

### Step 1:
```
ssh <src-node>
ssh-keygen -t rsa
cp ~/.ssh/id_rsa.pub src.key
scp src.key <dest-node>:/tmp/
```
### Step 2:
```
ssh <dest-node>
cat /tmp/src.key >> ~/.ssh/authorized_keys
```
