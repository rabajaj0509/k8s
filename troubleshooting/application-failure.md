Application Failure

a) Curl the endpoint with the node port to check for any issues.
$ curl http://web-service-ip:node-port

b) Check the service.
$ kubectl describe service web-service
check for the endpoints and correct selectors present in the pod
definition file

c) Check for the pod. Make sure it is in the running state.
$ kubectl describe pod web
$ kubectl log web -f previous

d) Check for the DB service and then check for the DB pod itself.
