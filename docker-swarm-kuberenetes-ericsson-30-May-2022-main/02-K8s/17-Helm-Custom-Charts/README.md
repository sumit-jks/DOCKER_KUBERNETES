```
1100  mkdir 17-Helm-Custom-Charts
 1101  cd 17-Helm-Custom-Charts/
 1102  ls
 1103  helm create mycharts
 1104  ls
 1105  cd mycharts/
 1106  ls
 1107  cat Chart.yaml
 1108  ls
 1109  ls -ltr templates/
 1110  ls
 1111  vim values.yaml
 1112  ls
 1113  cd ..
 1114  l
 1115  ls
 1116  helm install my-cus-nginx mycharts --dry-run
 1117  helm install my-cus-nginx mycharts
 1118  kubectl  get pods
 1119  kubectl  get svc
 1120  ls
 1121  helm create mypywebapp
 1122  ls
 1123  cd mypywebapp/
 1124  ls
 1125  vim values.yaml
 1126  ls
 1127  vim templates/deployment.yaml
 1128  ls
 1129  vim values.yaml
 1130  ls
 1131  cd ..
 1132  ls
 1133  helm install my-pyapp mypywebapp --dry-run
 1134  helm install my-pyapp mypywebapp
 1135  kubectl  get pods,svc
 1136  ls
 1137  history
 1138  helm list
 1139  helm uninstall my-pyapp
 1140  helm list
 1141  kubectl  get pods,svc
 1142* helm install my-cus-nginx-2 mychar
 1143  helm install my-cus-nginx-3 mycharts
 1144  helm install my-cus-nginx-4 mycharts
 1145  ls
 1146  helm list
 1147  ls
 1148  cd ..
 1149  ls
 1150  cp -rf 06-Deployments 18-Deploy
 1151  ls
 1152  kubectl  apply -f 18-Deploy/
 1153  kubectl  create  -f 18-Deploy/
 1154  ls
 1155  cd 17-Helm-Custom-Charts/
 1156  ls
 1157  cd mycharts/
 1158  ls
 1159  vim values.yaml
 1160  cd
 1161  helm repo list
 1162  helm repo add bitnami https://charts.bitnami.com/bitnami
 1163  helm repo list
 1164  helm  search repo nginx
 1165  helm install my-release bitnami/jenkins
 1166  kubectl get secret --namespace default my-release-jenkins -o jsonpath="{.data.jenkins-password}" | base64 -d
 1167  kubectl  get pods
 1168  helm list
 1169  helm uninstall my-cus-nginx-2 my-cus-nginx-3 my-cus-nginx-4 my-release mynginx nginx-1654343177
 1170  helm list
 1171  kubectl  get pods
 1172  kubectl  get svc
 1173  helm install my-release bitnami/jenkins
 1174  kubectl  get svc
 1175  kubectl  get pods
```
