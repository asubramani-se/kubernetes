cd api
docker build -t flask-api .
docker run -d -p 5000:5000 --name api-container  flask-api
 
cd ..
cd webapp
docker build -t webapp .
docker run -d -p 80:80 --name webapp-container webapp
 
cd ..
kubectl apply -f app.yaml
kubectl get deployments
kubectl get services
 
