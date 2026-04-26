# Laboratorio
# 🔐 Informe de Laboratorio – Ethical Hacking

---

## 🎯 Objetivos

### 🧩 Configuración del entorno

* Configurar un laboratorio de pruebas de penetración utilizando máquinas virtuales como **Kali Linux** y **Metasploitable 2**.
* Establecer comunicación entre máquinas mediante una red virtual controlada.

---

### 🔍 Reconocimiento

* Identificar hosts activos dentro de la red.
* Detectar puertos abiertos y servicios en ejecución mediante herramientas de escaneo.

---

### 💥 Explotación

* Identificar vulnerabilidades explotables en el sistema objetivo.
* Ejecutar ataques controlados para obtener acceso al sistema.

---

## 🧪 Procedimiento Experimental

---

### 🔹 Parte A – Configuración del entorno de laboratorio

1. Instalación o configuración de **Kali Linux**.
2. Importación o configuración de **Metasploitable 2**.
3. Configuración de red virtual entre las máquinas.
4. Verificación de conectividad mediante pruebas de red (ping).

---

### 🔹 Parte B – Reconocimiento y escaneo de red

1. Identificación de hosts activos dentro de la red.
2. Escaneo de puertos utilizando **Nmap**.
3. Identificación de servicios y versiones detectadas.

---

### 🔹 Parte C – Explotación de vulnerabilidades

1. Búsqueda de exploits dentro de **Metasploit**.
2. Configuración de parámetros del exploit.
3. Ejecución del exploit contra el sistema objetivo.
4. Obtención de acceso al sistema vulnerable.

---

### 🔹 Parte D – Post-explotación

1. Verificación de privilegios del usuario obtenido.
2. Obtención de información del sistema comprometido.
3. Identificación de posibles vectores adicionales de ataque.

---

## 📊 Resultados de la Práctica

* Resultados obtenidos durante el escaneo de red.
* Listado de puertos abiertos detectados.
* Servicios y versiones identificadas.
* Vulnerabilidades detectadas durante el análisis.
* Evidencia de la explotación realizada.
* Capturas de pantalla de las herramientas utilizadas.

---

## 📈 Análisis de Resultados

* Interpretación técnica de los resultados del escaneo de red.
* Análisis de las vulnerabilidades identificadas.
* Evaluación del impacto de seguridad de las vulnerabilidades explotadas.
* Propuesta de mecanismos de mitigación.
* Identificación de errores durante la práctica.
* Reflexión sobre la importancia del análisis de seguridad.

---

## 📌 Conclusiones

* El Ethical Hacking es fundamental para identificar vulnerabilidades en sistemas informáticos.
* Las pruebas de penetración permiten evaluar el nivel de seguridad de una infraestructura.
* Es crucial mantener los sistemas actualizados y correctamente configurados.
* La práctica permitió fortalecer habilidades en análisis de seguridad.
* Los conocimientos adquiridos son aplicables en entornos reales de ciberseguridad.
* ## 📊 Resultados de la Práctica

Durante la ejecución del laboratorio de Ethical Hacking en un entorno controlado, se obtuvieron los siguientes resultados:

### 🔍 Escaneo de red

Se realizó un escaneo utilizando la herramienta **Nmap**, logrando identificar un host activo dentro de la red:

* **Host detectado:** 192.168.56.101 (Metasploitable 2)

---

### 🔓 Puertos abiertos detectados

El escaneo reveló múltiples puertos abiertos en el sistema objetivo:

| Puerto | Servicio | Estado  |
| ------ | -------- | ------- |
| 21     | FTP      | Abierto |
| 22     | SSH      | Abierto |
| 23     | Telnet   | Abierto |
| 25     | SMTP     | Abierto |
| 80     | HTTP     | Abierto |
| 139    | NetBIOS  | Abierto |
| 445    | SMB      | Abierto |

---

### ⚙️ Servicios y versiones identificadas

Se identificaron servicios vulnerables ejecutándose en el sistema:

* FTP: vsftpd 2.3.4
* SSH: OpenSSH 4.7p1
* HTTP: Apache 2.2.8
* SMB: Samba 3.0.20

---

### ⚠️ Vulnerabilidades detectadas

Durante el análisis se identificaron vulnerabilidades conocidas:

* Servicio FTP vulnerable (vsftpd 2.3.4 backdoor)
* Uso de Telnet sin cifrado
* Versión antigua de Samba con posibles exploits
* Servicios innecesarios expuestos

---

### 💥 Explotación realizada

Se utilizó **Metasploit Framework** para explotar una vulnerabilidad en el servicio FTP:

* Módulo utilizado: `exploit/unix/ftp/vsftpd_234_backdoor`
* Resultado: acceso exitoso al sistema

Se obtuvo una sesión tipo shell en el sistema objetivo.

---

### 🖥️ Evidencia de acceso

Una vez comprometido el sistema, se logró:

* Ejecución de comandos básicos (`whoami`, `uname -a`)
* Navegación por el sistema de archivos
* Identificación del sistema operativo (Linux vulnerable)

---

### 📸 Evidencias

Durante la práctica se obtuvieron evidencias mediante capturas de pantalla de:

* Resultado del escaneo con Nmap
* Configuración y ejecución del exploit en Metasploit
* Acceso exitoso al sistema

---

## 📈 Análisis de Resultados

Los resultados obtenidos evidencian que el sistema objetivo presenta múltiples vulnerabilidades críticas.

### 🔎 Interpretación técnica

* La presencia de múltiples puertos abiertos incrementa la superficie de ataque
* Los servicios desactualizados representan riesgos significativos
* El uso de protocolos inseguros (Telnet) facilita la interceptación de datos

---

### ⚠️ Evaluación de vulnerabilidades

Las vulnerabilidades detectadas tienen un impacto alto debido a:

* Posibilidad de acceso no autorizado
* Ejecución remota de comandos
* Compromiso total del sistema

---

### 🛡️ Medidas de mitigación

Se recomienda:

* Actualizar servicios a versiones seguras
* Deshabilitar servicios innecesarios
* Implementar firewall para restringir accesos
* Utilizar protocolos seguros (SSH en lugar de Telnet)

---

### ❗ Errores identificados

* Configuración insegura del sistema objetivo
* Exposición innecesaria de servicios
* Falta de actualizaciones de seguridad

---

### 💡 Reflexión

La práctica demuestra la importancia de realizar auditorías de seguridad de manera periódica para identificar y corregir vulnerabilidades antes de que puedan ser explotadas.

---

## 📌 Conclusiones

* El Ethical Hacking permite identificar debilidades críticas en sistemas.
* Las pruebas de penetración son esenciales para mejorar la seguridad.
* Los sistemas desactualizados representan un alto riesgo.
* La correcta configuración y monitoreo reduce significativamente las amenazas.
* La práctica permitió aplicar conocimientos teóricos en un entorno realista.

---


---
<img width="956" height="527" alt="imagen - 2026-04-25T184813 583" src="https://github.com/user-attachments/assets/d4de7139-6264-446b-950e-9bfa0b9fd937" />
<img width="1683" height="265" alt="imagen - 2026-04-25T184824 330" src="https://github.com/user-attachments/assets/60f1e102-645f-4129-bdc9-e38bf4f76d95" />
<img width="988" height="715" alt="imagen - 2026-04-25T184824 329" src="https://github.com/user-attachments/assets/1595c4c8-df1b-42e1-9954-abbe4bb696b0" />
<img width="956" height="527" alt="imagen - 2026-04-25T184849 023" src="https://github.com/user-attachments/assets/093c088e-96d5-4461-88ad-833e83fc8ed7" />
<img width="988" height="715" alt="imagen - 2026-04-25T184853 319" src="https://github.com/user-attachments/assets/ceb356ad-ce3c-4b20-838e-8569a8d02d64" />
<img width="1007" height="802" alt="imagen - 2026-04-25T184857 049" src="https://github.com/user-attachments/assets/3f39e885-e747-4c5a-a424-37020e2a5a03" />
<img width="1017" height="788" alt="imagen - 2026-04-25T184900 513" src="https://github.com/user-attachments/assets/080cc73f-5196-4e6f-9a78-dcbc959cedac" />
<img width="992" height="218" alt="imagen - 2026-04-25T184903 975" src="https://github.com/user-attachments/assets/2e62bb34-9c66-4e22-b65c-20cc34a65290" />
<img width="1683" height="265" alt="imagen - 2026-04-25T184907 071" src="https://github.com/user-attachments/assets/22a82796-213e-40b6-a9a3-13e6979f082b" />
<img width="1747" height="650" alt="imagen - 2026-04-25T184911 696" src="https://github.com/user-attachments/assets/f81f19ca-33da-402c-bfe0-45eaeb24e3db" />
<img width="1115" height="212" alt="imagen - 2026-04-25T184916 291" src="https://github.com/user-attachments/assets/3084c3ae-1963-4389-9553-77c5fe427656" />
<img width="1907" height="609" alt="imagen - 2026-04-25T184920 594" src="https://github.com/user-attachments/assets/88ee9c5b-25ea-4be0-bbc8-61510ea88aac" />
<img width="1907" height="609" alt="imagen - 2026-04-25T184939 545" src="https://github.com/user-attachments/assets/694d8053-1e1b-4cf7-9017-452b0d4719b3" />
<img width="1714" height="552" alt="imagen - 2026-04-25T184947 350" src="https://github.com/user-attachments/assets/febafefa-6179-4a1a-8d67-19591b7df76d" />
