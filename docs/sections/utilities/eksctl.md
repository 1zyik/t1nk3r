icon: simple/amazoneks

!!! info
     This is not a subsititute for eksctl core documentation. <br>
     [EKS CTL documentation](https://eksctl.io/getting-started/)

## Create Cluster from manifest file
```
eksctl create cluster -f <filename.yaml>
```

## Delete Cluster from manifest file
```
eksctl delete cluster -f <filename.yaml>
```

## Scale up a cluster nodes directly from CLI
```
eksctl scale nodegroup --cluster [Cluster Name]--name [Nodegroup name] --nodes 2 --nodes-max 2 --nodes-min 1 
```

## See all Node Groups
```
eksctl get nodegroups --cluster <cluster-name>
```

## Delete Node groups
```
eksctl delete nodegroup --cluster <cluster-name>
```