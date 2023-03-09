## Commands

**Strictly** follow the below order.

1. Create secret first to be used by mongodb deployment --> `kubectl apply -f secret.yml` 

2. Now you can start the mongodb deployment and service --> `kubectl apply -f mongodb.yml`

3. Now create the config Map to be used by mongo-express later --> `kubectl apply -f configMap.yml`

4. Create mongo-express deployment and external service --> `kubectl apply -f mongo-express.yml`

If you are using minkube don't forget to run the below command to get the external IP where you can access the mongo-express UI
 
 `minikube service mongo-express-service`
