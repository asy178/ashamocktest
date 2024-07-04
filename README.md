Mock Test Asha

Check 1:
nano 1-StorageClass.yaml

Check 2:
kubectl create namespace qq3 --dry-run=client -o yaml > 2-namespace.yaml
kubectl apply -f 2-namespace.yaml
kubectl apply -f 2-pv.yaml -f 2-pvc.yaml -n qq3

Check 3:
kubectl create namespace qq2 --dry-run=client -o yaml > 3-namespace.yaml
kubectl apply -f 3-namespace.yaml
kubectl apply -f 3-pod.yaml -n qq2

Check 4:
--


Check 5:
nano 5-nginx.yaml
kubectl apply -f 5-nginx.yaml -n qq3


