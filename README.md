# Evaluacion-Formativa-Redes

🖥️ Evaluación Formativa - Implementación de Máquinas Virtuales

## 📌 Descripción
En esta evaluación se implementaron dos máquinas virtuales:

- Windows Server 2019 (con GUI)
- Linux (Kali Linux - modo CLI)

Se configuraron servicios de red y acceso remoto (RDP y SSH), además de verificar conectividad mediante direcciones IP.

---

# ⚙️ 1. Creación de entorno

Se utilizó un software de virtualización (VirtualBox / VMware) para la creación de las máquinas virtuales.

---

# 🪟 2. Windows Server 2019

## 🔹 Configuración de la VM
- RAM: 8 GB
- Disco: 30 GB
- CPU: 2 vCPU
- Sistema: Windows Server 2019 Datacenter Evaluation (Desktop Experience) 

---

## 🔹 Verificación de dirección IP

Se utilizó el siguiente comando en CMD:

-  ipconfig

## 🔹 Habilitación de Escritorio Remoto (RDP)

Para permitir el acceso remoto al servidor, se habilitó la opción de Escritorio Remoto desde la configuración del sistema.

### Método utilizado:
1. Ir a:
   - **Configuración**
   - **Sistema**
   - **Escritorio remoto**
2. Activar la opción:
   - ✅ "Habilitar Escritorio remoto"
3. Confirmar los cambios


---

## 🔹 Verificación del servicio RDP

Debido a limitaciones del entorno (uso de ISOs y configuración de laboratorio), no fue posible realizar una conexión remota desde otro equipo.

Sin embargo, se verificó correctamente:

- Activación del Escritorio Remoto en el sistema  
- Configuración del servicio utilizando el puerto por defecto **3389**


# 🐉 3. Kali Linux (CLI)

## 🔹 Configuración de la máquina virtual
Se creó una máquina virtual con las siguientes características:

- RAM: 8 GB  
- Disco: 30 GB  
- CPU: 2 vCPU  
- Sistema operativo: Kali Linux (modo CLI)

---

## 🔹 Verificación de dirección IP

Para verificar la dirección IP de la máquina, se utilizó el siguiente comando:

-ip a

## 🔹 Configuración de acceso SSH

Para habilitar el acceso remoto, se instaló y configuró el servicio SSH.

Instalación y configuración:
- sudo apt update
- sudo apt install openssh-server -y
- sudo systemctl start ssh
- sudo systemctl enable ssh

Verificación del servicio:
- sudo systemctl status ssh

Se comprobó que el servicio se encuentra activo y en ejecución.

## 🔹 Observación

Debido a limitaciones del entorno de laboratorio, no fue posible realizar pruebas de conexión remota desde otro equipo.

Sin embargo, se verificó correctamente:

- Servicio SSH instalado
- Servicio activo y habilitado
- Puerto 22 en estado de escucha
## ✅ Resultado
- Dirección IP verificada
- Servicio SSH operativo
- Puerto 22 habilitado para conexiones remotas

## 📁 Evidencia

En las carpetas del repositorio se encuentra la documentación y evidencia (capturas) del proceso realizado en la evaluación.
