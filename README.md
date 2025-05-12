# 🚀 Desafío 13: Despliegue de ArgoCD en Minikube

## 📋 Descripción

Este proyecto consiste en desplegar una aplicación usando ArgoCD en un entorno local con Minikube. El objetivo es integrar una aplicación desde un repositorio Git mediante ArgoCD y automatizar el despliegue en un clúster Kubernetes.

# 💻 Tecnologías Utilizadas

🐳 Minikube: Herramienta para ejecutar Kubernetes localmente.

📦 Kubectl: Herramienta de línea de comandos para interactuar con clústeres de Kubernetes.

🌐 ArgoCD: Plataforma de GitOps para despliegues continuos en Kubernetes.

🗃️ GitHub: Almacenamiento de código fuente y versionado.

💾 Docker: Contenerización de aplicaciones.

## 🛠️ Requisitos

Minikube instalado 🟢

Kubectl instalado 🟢

Acceso administrativo para ejecutar comandos

GitHub para almacenar el repositorio

## ⚙️ Instalación de Minikube
En mi caso ya lo tenia instalado en mi maquina local 

![image](https://github.com/user-attachments/assets/74ec47eb-1f79-4823-9e1b-d781862c39bc)

## 🧰 Instalación de Kubectl

En mi caso ya lo tenia instalado en mi maquina local 

![image](https://github.com/user-attachments/assets/b2188c3e-b61b-431b-bd0b-0d8606818412)

## 🚦 Despliegue de ArgoCD en Minikube

1️⃣ Iniciar Minikube

![image](https://github.com/user-attachments/assets/2b842d22-8b42-426f-9590-fc7e6c54fbe2)

2️⃣ Crear el namespace para ArgoCD

![image](https://github.com/user-attachments/assets/2fce0015-cd04-4eba-84e9-c68266521e76)

3️⃣ Desplegar ArgoCD usando los manifiestos oficiales

![image](https://github.com/user-attachments/assets/ee599002-299d-4fd4-a5ad-5b3e92dcc87e)

4️⃣ Verificar el despliegue

![image](https://github.com/user-attachments/assets/2c45ace5-2c6f-4095-8d4c-4686c2bc3cce)

# 🔧 Configuración de ArgoCD

🌐 Exponer el servicio ArgoCD Server

![image](https://github.com/user-attachments/assets/cc705f7d-db64-4997-89d0-ca6df256d0a3)

🔑 Obtener la contraseña inicial

![image](https://github.com/user-attachments/assets/5a1b2832-8645-4b87-8e72-22097f61078b)

# 🌱 Conectar ArgoCD con un Repositorio Git

💻 Acceder al dashboard
Abrir el navegador e ir a:

```
https://localhost:8080
```
📝 Crear una aplicación desde el dashboard
```
1. Hacer clic en New App.

2. Completar el formulario con los siguientes datos:

    Application Name: educacionit-app

    Project: default

    Sync Policy: Automatic

    Repository URL: https://github.com/gaboibarra/Desafio13.git

    Revision: HEAD

    Path: .k8s

    Cluster: https://kubernetes.default.svc

    Namespace: default

3. Hacer clic en Create para guardar.
```

1️⃣ Dashboard de ArgoCD

![image](https://github.com/user-attachments/assets/6d03420e-d2ae-4d9d-a1b9-7f50b4c26b59)

2️⃣ Creacion de la app

![image](https://github.com/user-attachments/assets/40cb5bcd-54d5-4fbf-b33b-132f25e1ce4d)

![image](https://github.com/user-attachments/assets/291efb65-44d9-48ce-803b-6f13cafe0468)

3️⃣ App desplegada

![image](https://github.com/user-attachments/assets/17edfd40-2592-4c9f-adae-916f43a0ff53)

## 📝 Autor

Gabriel Ibarra
