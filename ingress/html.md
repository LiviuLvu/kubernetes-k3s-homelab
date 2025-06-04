Test nginx page load using a temporary config map:  
k3 create configmap mysite-html --from-file=./index.html
