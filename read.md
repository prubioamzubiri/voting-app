# Aplicación de Votación

Esta es una aplicación simple de votación que permite a los usuarios votar entre dos opciones. La aplicación está containerizada y diseñada para ejecutarse en Kubernetes.

## Despliegue

Para desplegar la aplicación usando kubectl, sigue estos pasos:

1. Aplica todos los manifiestos de Kubernetes:
```bash
kubectl apply -f .
```

2. Verifica el despliegue:
```bash
kubectl get pods
kubectl get services
```

La aplicación consiste en varios microservicios que se desplegarán en tu clúster de Kubernetes. Una vez desplegada, podrás acceder a la interfaz de votación a través del endpoint del servicio.

## Componentes

- Frontend de votación
- Frontend de resultados
- Base de datos Redis
- Base de datos Postgres
- Servicio Worker