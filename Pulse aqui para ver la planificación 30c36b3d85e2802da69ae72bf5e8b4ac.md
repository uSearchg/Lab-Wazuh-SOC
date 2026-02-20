# Pulse aqui para ver la planificación

### Arquitectura y topología:

- Usaremos un SIEM server en nuestro caso una OVA  de Wazuh  [https://documentation.wazuh.com/current/deployment-options/virtual-machine/virtual-machine.html](https://documentation.wazuh.com/current/deployment-options/virtual-machine/virtual-machine.html) la cual usaremos como cerebro del proyecto
- Como victima o Endpoint un windows 11
- Como atacante un Kali Linux [https://www.kali.org/get-kali/](https://www.kali.org/get-kali/)

### Despliegue:

- Importaremos la OVA y le asignaremos los recursos en el virtualbox
- Configuraremos el servidor en nuestro caso con credenciales admin/admin

- Despliegue del agente:
    - Descargar ISO windows 11 [https://www.microsoft.com/es-es/software-download/windows11](https://www.microsoft.com/es-es/software-download/windows11)
    - Vincular IP servidor
    - Verificar que el agente aparece como Activo

![image.png](image%2022.png)

### Ejecución:

- Escaneo y reconocimiento( usaremos Nmap desde el kali
- Ataque a fuerza bruta con el uso de hydra
- Alteracion y modificacion de un archivo critico para que el FIM lo detecte