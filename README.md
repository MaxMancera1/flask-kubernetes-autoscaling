# 🚀 Flask + Kubernetes + Autoscaling

Este proyecto es una aplicación web simple escrita en **Python (Flask)** y desplegada en **Kubernetes (Minikube)** con configuración de **autoscaling** (HPA).

## 📦 Características

- ✅ App "Hola Mundo" con Flask
- 🐳 Dockerfile para contenedorizar la app
- ☸️ Despliegue con Kubernetes + Minikube
- 🔄 Autoscaling (HPA): 2 pods mínimos, hasta 4 máximos
- 📈 Escala automáticamente si sube el uso de CPU

## 🧱 Estructura del proyecto


## ⚙️ Cómo desplegar en Minikube

```bash
# 1. Iniciar Minikube
minikube start

# 2. Desplegar recursos
kubectl apply -f k8s/

# 3. Exponer la app
minikube service hello-python-service

