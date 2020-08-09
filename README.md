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
