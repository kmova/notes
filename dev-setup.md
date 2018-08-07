
```
sudo apt-get update
sudo apt-get install golang git psmisc jsonlint yamllint gcc curl socat
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
```

```
sudo apt-get update
sudo apt-get install socat
curl -Lo kubectl https://storage.googleapis.com/kubernetes-release/release/v1.9.4/bin/linux/amd64/kubectl && chmod +x kubectl && sudo mv kubectl /usr/local/bin/
curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 && chmod +x minikube && sudo mv minikube /usr/local/bin/
chmod 700 get_helm.sh
./get_helm.sh 
```

```
~/go/src/github.com/kmova/bootstrap/gke-gcloud/setup.sh
```

