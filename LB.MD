```
kubectl apply -f https://raw.githubusercontent.com/google/metallb/v0.8.3/manifests/metallb.yaml

```
```
kubectl get ns
```
```
kubectl get all -n metallb-system
```
![image](https://user-images.githubusercontent.com/45539698/73608480-6f95b480-45e9-11ea-8116-5225a32b9c86.png)
![image](https://user-images.githubusercontent.com/45539698/73608507-ed59c000-45e9-11ea-8210-66596cfd285c.png)

Create a cm

[root@master K8Experiments]# cat lbconfigmap.yml 

```
apiVersion: v1
kind: ConfigMap
metadata:
  namespace: metallb-system
  name: config
data:
  config: |
    address-pools:
    - name: default
      protocol: layer2
      addresses:
      - 192.168.152.150-192.168.152.160
```
