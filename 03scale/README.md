scaling 테스트

kubectl create deployment httpd-deployment --image=httpd:latest

[centos@shi-kubectl yaml]$ kgdep
NAME               READY   UP-TO-DATE   AVAILABLE   AGE
httpd-deployment   1/1     1            1           104s

$ kubectl get rs
NAME                         DESIRED   CURRENT   READY   AGE
httpd-deployment-9579fb846   1         1         1       2m12s

 the name of the ReplicaSet is always formatted as [DEPLOYMENT-NAME]-[RANDOM-STRING]


$ kubectl scale deployments/httpd-deployment --replicas=4
deployment.extensions/httpd-deployment scaled
[centos@shi-kubectl yaml]$ kgdep
NAME               READY   UP-TO-DATE   AVAILABLE   AGE
httpd-deployment   3/4     4            3           4m6s
[centos@shi-kubectl yaml]$ kgdep
NAME               READY   UP-TO-DATE   AVAILABLE   AGE
httpd-deployment   4/4     4            4           4m9s




