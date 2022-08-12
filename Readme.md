# This project conatins file for simple demonstartion of 3 diffrent Docker containers controlled by Nginx load balancer.

The whole project is set-up using docker compose.

Note: To run this project you can run cmd `docker-compse up`

ff1b4be433eb   nginx-as-load-balancer_nginx          "/docker-entrypoint.…"   52 minutes ago      Up 51 minutes      0.0.0.0:9000->80/tcp                                       nginx-as-load-balancer-nginx-1
00766c1d4dee   nginx-as-load-balancer_app1           "python3 app1.py"        52 minutes ago      Up 51 minutes                                                                 nginx-as-load-balancer-app1-1
1a3517454b44   nginx-as-load-balancer_app2           "python3 app2.py"        52 minutes ago      Up 51 minutes                                                                 nginx-as-load-balancer-app2-1
90c6cde47494   nginx-as-load-balancer_app3           "python3 app1.py"        52 minutes ago      Up 51 minutes                                                                 nginx-as-load-balancer-app3-1

Uploaded to Docker Hub
===================================================================================================================

docker tag nginx-as-load-balancer_nginx bipin115/nginx-loadbalancer
docker image push bipin115/nginx-loadbalancer

docker tag nginx-as-load-balancer_app1 bipin115/py-test-app-01
docker image push bipin115/py-test-app-01

docker tag nginx-as-load-balancer_app2 bipin115/py-test-app-02
docker image push bipin115/py-test-app-02

docker tag nginx-as-load-balancer_app3 bipin115/py-test-app-03
docker image push bipin115/py-test-app-03



IMAGES UPLOADED on DOCKER HUB
============================================================================================

bipin115/py-test-app-03
bipin115/py-test-app-02
bipin115/py-test-app-01
bipin115/nginx-loadbalancer

