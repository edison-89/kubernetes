"# kubernetes" 


# DEPLOYMENTS

# Aplicar el manifiesto
kubectl apply - f dep.yaml

# Ver el deployment
kubectl get deployment

# Mostrar los labels de un deployment
kubectl get deployment --show-labels

# Nos cuenta que paso con el deployment ('deployment-test' es el nombre de mi deployment de prueba)
kubectl rollout status deployment deployment-test


