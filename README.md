# Tips to generate yaml files


**Auto complete kubectl**
```
alias k=kubectl
complete -F __start_kubectl k
```
__Generate yaml tips:__
```
This generate the yaml complete structure and helps to build jsonpath

kubectl explain Pod --recursive  | cut -d '<' -f1 | cut -d ' ' -f4-
or

k explain Pod --recursive  | cut -d '<' -f1 | cut -d ' ' -f4-
```
__Set New Editor__
```
Be default k8s comes with vi editor during edit ie- kubectl edit <resource> <resource name>. Updating KUBE_EDITOR  can set the new editor of our choice

export KUBE_EDITOR=nano
this sets for the session

for temporary

KUBE_EDITOR=nano kubectl edit <resource> <resource name>
```

