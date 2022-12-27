"# kubernetes" 
# PODS

# Para ver descripción detallada de los pods
kubectl get pods -l app=ront -o wide



# DEPLOYMENTS

# Aplicar el manifiesto
kubectl apply - f dep.yaml

# Ver el deployment
kubectl get deployment

# Mostrar los labels de un deployment
kubectl get deployment --show-labels

# Nos cuenta que paso con el deployment ('deployment-test' es el nombre de mi deployment de prueba)
kubectl rollout status deployment deployment-test

# Para ver el historial de un deployment especifico
kubectl rollout history deployment deplyment-test

# Para revisar una versión(revisión) especifica del historico
kubectl rollout history deployment deplyment-test --revision=2

# Realizar un rollback a una versión (revisión) especifica
kubectl rollout undo deployment deployment-test --to-revision=3


# SERVICE

# Aplicamos el maniiesto del service
kubectl apply - svc.yaml

# Listar los servicios
kubectl get svc

# Describir la coniguración de un servicio
kubectl describe svc my-service
