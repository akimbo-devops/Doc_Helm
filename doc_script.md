# Install helm
- curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3
- chmod 700 get_helm.sh
- ./get_helm.sh

# Example for upgrade pod using helm
- helm list -A
- helm upgrade namepacakge namerepo/package -f filevalues.yaml -n namanamespace --version "versi chart"
* helm upgrade prometheus prometheus-community/prometheus -f values-prometheus.yaml -n monitoring  --version 14.11.0
- Note: has to include the version, because if we didn't include that, the version maybe will change and maybe some of configuration will fail. 

# Random (Just arrange this when I wanna do that :D)
- helm search repo grafana
