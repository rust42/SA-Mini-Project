<b>Mini Project2</b>

Software Installation Prerequisites

1) `Docker`
2) `minikube` | `kind` | `k3d`

<b>Download the project, unzip and goto project folder</b>.

To run this project using kubernetes. Goto setup folder `cd setup`

and change permission of the startup sh using `chmod +x start.sh`

then run project using `./start.sh`

In this Project, We have a 6 services.

<b>1) Product Service<br/>
2) Order Service <br/>
3) Address Service(used for billing and shipping address)<br/>
4) Transaction Service<br/>
5) Payment Services<br/>
6) Authorization Service</b>

<b>Database</b> -> `MySQL`

Programming Language -> `Spring boot, Spring cloud`

After running project you can check the pods, services, ingress controller, logs by using following command.

to view list of the pods. `kubectl get pods`

to view list of the services `kubectl get svc`

To view logs `kubectl logs pod-name`

to view ingress `kubectl get ingress`

to view configmap list `kubectl get configmap `
to view secrets `kubectl get secrets`



for deleting all the pods,services, ingress, configmap, secret
goto setup folder and enter following command. `chmod +x delete.sh && ./delete.sh`
