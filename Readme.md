# docker push csc111vs/hello-node:latest
1. docker run -p 8000:3000 --name nodeapp 2dddf
2. docker stop ddebb
3. docker run -it --name pythonapp bmi
4. docker stop nodeapp
5. docker ps -a
6. docker start-ia pythonapp
7. docker rm nodeapp pythonapp
8. docker rmi bmi bmi
9. docker images prune -a
10. docker system prune -a
11. docker build -t hello-node:latest .
12. docker build -t bmi-app:1.0.0 .
13. docker run -p 8000:3000 -d --name node-demo --rm hello-node
14. docker stop node-demo
15. docker run -it --name python-demo --rm bmi-app:1.0.0
docker push csc111vs/hello-node:tagname
1. docker tag hello-node:latest csc111vs/hello-node:latest
2. docker push csc111vs/hello-node:latest
# Volumes
1. docker run  -p 8000:80 -d --name feedback-app --rm  -v feedback:/app/feedback  -v "C:\Users\sarath_chintapatla\sarath_workspace\github\2021\Cubes\assignment-problem\data-volumes-01-starting-setup:/app" -v /app/node_modules feedback-node:volume
2. Powershell :  docker run  -p 8000:80 -d --name feedback-app --rm  -v feedback:/app/feedback  -v "${PWD}:/app" -v /app/node_modules feedback-node:volume
3. CMD prompt :  docker run  -p 8000:80 -d --name feedback-app --rm  -v feedback:/app/feedback  -v "%cd%:/app" -v /app/node_modules feedback-node:volume
4. Linux :  docker run  -p 8000:80 -d --name feedback-app --rm  -v feedback:/app/feedback  -v "$(PWD):/app" -v /app/node_modules feedback-node:volume
5. 