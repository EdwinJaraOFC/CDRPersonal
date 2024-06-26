<p align="left">
  <img src="https://semanadelcannabis.cayetano.edu.pe/assets/img/logo-upch.png" width="150">
  <h1 align="center">Actividad 1: Creación de una red simple</h1>
</p>

## Tabla de direccionamiento

<p align= "center">
  <img src="https://github.com/EdwinJaraOFC/CDRGrupo5/assets/150296803/5113ce59-074a-41af-ab72-f77504316a8a">
</p>

## Paso 1: Construye la red simple configurando cada uno de los dispositivos dados.
<p align= "justify">
  
1. En la interfaz de Packet Tracer selecciona los dispositivos dados: Switch 2960.
2. Click en el dispositivo y en la pestaña Config, Display Name, Hostname Cambia el nombre a S1.
3. Realiza el mismo procedimiento para los otros dispositivos. Llamalos PC-A, PC-B respectivamente
4. Selecciona el ícono Rayo de conexiones y escoge Copper Straight-Through.
5. Conecte un extremo de un cable Ethernet al puerto de NIC en PC-A. Conecte el otro extremo del cable a F0/6 en S1. Después de conectar la PC al switch, la luz de F0/6 debería tornarse ámbar y luego verde.
6. Conecte un extremo de un cable Ethernet al puerto de NIC en PC-B. Conecte el otro extremo del cable a F0/1 en S1. Después de conectar la PC al switch, la luz de F0/1 debería tornarse ámbar y luego verde.
</p>
<p align= "center">
  <img src="https://github.com/EdwinJaraOFC/CDRGrupo5/assets/150296803/bb6b0c33-0db4-4149-afbb-e82ca78e8524" alt="Grupo trabajando" />
</p>

## Paso 2: Verifique la configuración y la conectividad de la PC.
<p align= "justify">

1. Desde PC-A, haga clic y Desktop seleccione **Command Prompt.**
2. En la ventana de comandos de packet tracer, verifique la configuración de la PC mediante el comando ipconfig /all.
</p>
<div align="center"; style="display: flex; justify-content: space-between;">
  <img src="https://github.com/EdwinJaraOFC/CDRPersonal/assets/150296803/cc8c24e7-76cd-4475-92f2-ce675635f3ab" width="500px">
  <img src="https://github.com/EdwinJaraOFC/CDRPersonal/assets/150296803/24319b4a-fa2f-4a47-a0a6-3a694219498a" width="500px">
</div>
<p align= "justify">
  
3. Escriba ping 192.168.1.11 y presione Intro. **¿Fueron correctos los resultados del ping?** <br>- Sí, se enviaron y recibieron los paquetes de manera correcta.
4. Repite los pasos anteriores para PC-B **¿Fueron correctos los resultados del ping?** <br>- Sí, igualmente, se recibieron los mensajes en un tiempo adecuado.
</p>
<div align="center"; style="display: flex; justify-content: space-between;">
  <img src="https://github.com/EdwinJaraOFC/CDRPersonal/assets/150296803/36a03460-f419-4d66-aaf0-f5db797fbaf0" width="510px">
  <img src="https://github.com/EdwinJaraOFC/CDRPersonal/assets/150296803/ddb474f0-2486-4d3b-9d06-1979c6edffef" width="486px">
</div>
