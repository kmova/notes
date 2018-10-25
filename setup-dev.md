
```
sudo apt-get update
sudo apt-get install golang git psmisc jsonlint yamllint gcc curl socat
sudo apt install docker.io
sudo apt install open-iscsi
```

```
git config --global user.name "kmova"
git config --global user.email "kiran.mova@mayadata.io"
git config --global core.pager "less -r"
git config -l
```

```
sudo apt-get install golang-1.9-go

mkdir -p go/bin
mkdir -p go/src/github.com/kmova
mkdir -p go/src/github.com/openebs


cd go/src/github.com/kmova
git clone https://github.com/kmova/bootstrap.git
cd

#vi ~/.profile
#PATH="/usr/lib/go-1.9/bin:$PATH"
#GOROOT="/usr/lib/go-1.9"; export GOROOT
#GOPATH=$HOME/go; export GOPATH
#PATH=$PATH:$GOPATH/bin; export PATH
#PATH=$PATH:"/home/kiran/go/src/github.com/kmova/bootstrap/git"
#PATH="$HOME/go/src/github.com/kmova/bootstrap/gke-openebs/hack:$PATH"
#PATH="$HOME/go/src/github.com/kmova/bootstrap/gke-gcloud:$PATH"
```

```
sudo apt-get update
sudo apt-get install socat

~/go/src/github.com/kmova/bootstrap/minikube/setup-minikube.sh


curl https://raw.githubusercontent.com/kubernetes/helm/master/scripts/get > get_helm.sh
chmod 700 get_helm.sh
./get_helm.sh 
```

```
~/go/src/github.com/kmova/bootstrap/gke-gcloud/setup.sh
```

```
# Add to ~/.bash_aliases
# src aliases
alias cdgbs='cd $GOPATH/src/github.com/kmova/bootstrap/'
alias cdgmaya='cd $GOPATH/src/github.com/openebs/maya/'
alias cdgprov='cd $GOPATH/src/github.com/kubernetes/external-storage/'
alias cdgndm='cd $GOPATH/src/github.com/openebs/node-disk-manager/'
```
