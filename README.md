Mock Test Asha

Check 1:
nano 1-StorageClass.yaml

Check 2: 
kubectl create namespace qq3 --dry-run=client -o yaml > 2-namespace.yaml
kubectl apply -f 2-namespace.yaml
kubectl apply -f 2-pv.yaml -f 2-pvc.yaml -n qq3
