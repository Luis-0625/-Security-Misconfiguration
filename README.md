# -Security-Misconfiguration
Mediante OWAS-ZAP se escanean errores en la configuración de un sistema, aplicación o red que crea una vulnerabilidad de seguridad, permitiendo el acceso no autorizado.
# 🔒 Escaneo de seguridad con OWASP ZAP en un servidor Apache local

Este repositorio explica cómo configurar un servidor **Apache local** y usar **OWASP ZAP** para realizar pruebas de seguridad en aplicaciones web en entorno local.

---

## 🧠 Objetivo
Aprender a:
1. Instalar y configurar Apache localmente.
2. Instalar y usar OWASP ZAP.
3. Configurar un proxy entre ZAP y el navegador.
4. Ejecutar un escaneo de vulnerabilidades en una app local.

---

## 🧩 Requisitos
- 🧰 **Apache2** – Servidor web local.
- 🕵️ **OWASP ZAP** – Herramienta de análisis de seguridad.
- 🧑‍💻 **Navegador (Firefox o Chrome)** – Configurado con proxy manual.

---

## ⚙️ Instalación

### 1. Instalar Apache

sudo apt update
sudo apt install apache2

### 2. inicializa Apache

sudo systemctl start apache2

### 3. verificacion Apache
sudo systemctl status apache2

### 4 Instalar Owasp zap

sudo snap install zaproxy --classic


## 🔍 Escaneo de la aplicación local

### Inicia OWASP ZAP

En “Quick Start”, coloca la URL de tu Apache local:

http://localhost

Click en Attack

Observa el panel de alertas — verás vulnerabilidades clasificadas por nivel (High, Medium, Low, Informational).


