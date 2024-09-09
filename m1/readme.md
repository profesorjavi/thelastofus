### Misión1: **"El Enlace Vital. Parte 1"**

#### Contexto:
En el mundo post-apocalíptico de "The Last of Us", los supervivientes se han agrupado en pequeñas zonas de cuarentena para protegerse y sobrevivir. El poblado en el que se os encontráis, conocido como **"Zona de Cuarentena Alpha"**, dispone de conexión a internet. Sin embargo, el poblado vecino, **"Zona de Cuarentena Beta"**, aunque tiene la infraestructura necesaria, no puede acceder a internet. Para que la Zona de Cuarentena Beta pueda conectarse a internet, debéis configurar un dispositivo en la Zona de Cuarentena Alpha para que funcione como router.

En un mundo donde la comunicación es vital para la supervivencia, los héroes de la Zona de Cuarentena Alpha deben extender su red para ayudar a sus vecinos en la Zona de Cuarentena Beta. Con cada conexión establecida, no solo fortalecen su propia seguridad, sino que también crean un lazo de esperanza y colaboración en un mundo devastado. ¿Estáis listos para aceptar el desafío y convertir a la Zona de Cuarentena Beta en un aliado conectado?

#### Instrucciones:

1. **Preparación de las Máquinas Virtuales:**
   - **Ubuntu Server (US):** Esta máquina funcionará como el enrutador en la Zona de Cuarentena Alpha. Debe tener un adaptador puente de red y un adaptador de red en red interna.
   - **Ubuntu Desktop (Xubuntu):** Esta máquina se encontreá en la Zona de Cuarentena Beta y debe tener un adaptador en red interna.

2. **Paso 1: Configuración de IP Estática**
   - **Ubuntu Server (US):** Configura la IP estática del adaptador de red interna modificando el archivo de netplan.
   - **Xubuntu:** Configura la IP estática del adaptador de red interna utilizando la interfaz gráfica.
   - **Verificación:** Comprueba la conectividad haciendo un ping entre ambas máquinas.

3. **Paso 2: Verificación del Adaptador Puente**
   - **Ubuntu Server (US):** Asegúrate de que el adaptador puente funciona correctamente. Haz un ping desde el servidor a la máquina anfitrión.

4. **Paso 3: Configuración del Enrutador**
   - **Tutorial:** Revisa el video tutorial proporcionado. https://youtu.be/fO-n3vbdBY8
   - **Modificación:** Modifica el parámetro indicado en el tutorial para que US funcione como enrutador.

5. **Paso 4: Comprobación del Funcionamiento**
   - **Xubuntu:** Desde la máquina de Xubuntu, haz un ping a la IP de la interfaz del adaptador puente de la máquina US para comprobar que la configuración es correcta.

#### Nombres de los Dispositivos:
- **Ubuntu Server (US):** **"RAlpha"**
- **Xubuntu:** **"CBeta1"**

5. **Revisión del Concepto de NAT:**
   - **Video Tutorial:** Mira el video tutorial proporcionado y repasa el concepto de NAT (Network Address Translation). Este concepto es fundamental para permitir que múltiples dispositivos en la Zona de Cuarentena Beta accedan a internet a través del Enrutador Alpha.

6. **Configuración de DNS:**
   - **DNS Conselleria:** Configura los DNS en la interfaz de red de los equipos clientes en la Zona de Cuarentena Beta. Utiliza las siguientes direcciones DNS:
     - **Primario:** 10.239.3.7
     - **Secundario:** 10.239.3.8

7. **Configuración Persistente de NAT:**
   - **Persistencia:** Asegúrate de que la configuración de NAT quede de manera persistente en el Enrutador Alpha. Esto garantizará que la conexión a internet se mantenga estable y no se pierda tras un reinicio.
   - **Tutorial:** Sigue las instrucciones del tutorial en el siguiente enlace para configurar NAT de manera persistente: [Tutorial de NAT](https://youtu.be/sGdhakDeQyo).

8. **Verificación del Funcionamiento:**
   - **Prueba de Conexión:** Desde un equipo cliente en la Zona de Cuarentena Beta, realiza pruebas de navegación para asegurarte de que pueden acceder a internet correctamente.
   - **Ping:** Realiza un ping a una dirección externa (por ejemplo, 8.8.8.8) para verificar la conectividad.

# Repaso de redes
