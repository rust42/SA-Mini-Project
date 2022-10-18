<b>Mini Project2</b>

Software Installation Prerequisites

1) `Docker`
2) `minikube` | `kind` | `k3d`

<b>Download the project, unzip and goto project folder</b>.

If using minukube on mac, You have to run the following commands:

1. minikube addons enable ingress
2. minikube addons enable ingress-dns
3. minikube tunnel

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


`To see output and working flow of the project, you need to import postman collection in your postman app. then do following operation.`

<b>working flow:</b>

Login using `{{BASE_URL}}/api/auth/login`

Steps for the overall process:

1. Add Category to add the products, As product depends upon the category
2. Add Product, It accepts the category id
3. For adding the payment method, There are 3-different payment methods,  The address must be added.
4. Add the address and then the payment method.
5. Add any type of items and any number of it to the cart
6. Select the payment checkout option.
7. This will take order id and address id and the process is complete.   
