Mini Project2


Software Installation Prerequisites

1) Docker
2) minikube | kind | k3d


Download the project, unzip and goto project folder.

To run this project using kubernetes. Goto setup folder 
cd setup

and change permission of the startup sh using chmod +x start.sh


then run project using ./start.sh

In this Project, We have a 6 services.

1) Product Service
2) Order Service
3) Address Service(used for billing and shipping address)
4) Transaction Service
5) Payment Services
6) Authorization Service

Database -> MySQL

Programming Language -> Spring boot, Spring cloud


After running project you can check the pods, services, ing