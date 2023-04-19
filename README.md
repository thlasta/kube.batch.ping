echo "# kube.batch.ping" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:thlasta/kube.batch.ping.git
git push -u origin main

git pull git@github.com:thlasta/kube.batch.ping.git

# Namespace "batch" anlegen
kubectl create namespace batch