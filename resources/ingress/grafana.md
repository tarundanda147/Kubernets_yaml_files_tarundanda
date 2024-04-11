for grafana first create a configmap for the defaults.ini file which will be present in the grafana pod
first cp that file from grafana pod to the master using "kubectl cp pod-name:path-of-defaults.ini defaults.ini"
then open that file and change as following

# The full public facing url
root_url = %(protocol)s://%(domain)s:%(http_port)s/grafana/

# Serve Grafana from subpath specified in `root_url` setting. By default it is set to `false` for compatibility reasons.
serve_from_sub_path = true

then create a configmap using "kubectl create configmap grafana-conf-new --from-file=defaults.ini"
now we can apply the grafanadepl.yml file , now we should be able to access the grafana using loadbalancer DNS/grafana
