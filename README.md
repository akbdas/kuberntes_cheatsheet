# kuberntes_cheatsheet
Tips to generate yaml files

Generate yaml tips:

kubectl explain Pod --recursive  | cut -d '<' -f1 | cut -d ' ' -f4-


Auto complete kubectl

aliask=kubectl
complete -F __start_kubectl k
