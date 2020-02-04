Dynamic:

1. pvc requested by user
2. kubernetes will check sc, storage pods(system level)
3. pvc will be created(Pending) & pv will be requested 
4. storage server recieves request to create volume(pv)
5. storage server creates volume & give back to k8s.. PV is created 
6. PVC will be Bound state.
kishore bjv
1:06 PM
￼

static:

1. PV requested by user
  a. without sc -- user will mention target storage details,path
  b. with sc -- mention path

2. storage server recieves request to create volume(pv)
 
3. PV created by storage

4. PVC will be created by user

5. PVC will be Bound state.
1:11 PM
￼

https://github.com/rahulvaish/ReferenceDocuments/blob/master/UnderstandingKubernetes/%5B23%5D%20Kubernetes-LoadBalancing.MD
kishore bjv
1:22 PM
￼

DNS godaddy
public IP from ISP
public ip with dns map(in godaddy console)




router(public ip:(port range) =>> 192.168.152.150)
kishore bjv
1:23 PM
￼

router(public ip:80 =>> 192.168.152.150:8080)
kishore bjv
1:24 PM
￼

https://www.heroku.com/
