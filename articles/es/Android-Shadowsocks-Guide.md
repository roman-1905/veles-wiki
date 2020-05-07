Name:               Guía de Shadowsocks en Android para Veles
Image:              images/download/linux-wallet.png
GuideType:          Guía de Usuario
OS:                 Android
VelesdApp:          dVPN
Protocol:           Shadowsocks
Requirements:       cliente Shadowsocks
Difficulty:         Fácil
EstimatedTime:      5 minutos

# Guía de Shadowsocks para Android
Esto te guiará a través del proceso de instalar y utilizar Shadowsock en la plataforma Android.  

Si requiere más ayuda por favor contacte a nuestro equipo de soporte @ [Discord](https://discord.gg/P528fGg) 

## Requirimientos
1) **Instalar el cliente de Shadowsocks**  
2) **Descargar la configuración de OpenVPN para Veles**  

## Contenido
* **Sección A**: Descargar e instalar Shadowsocks
* **Sección B**: Configurar Shadowsocks
* **Sección C**: Conectarse a la dVPN de Veles con Shadowsocks
* **Sección D**: Testear la conexión Shadowsocks 
***

### Sección A: Descargar e instalar Shadowsocks

***Paso 1***

* Abrir **Google Play Store**. Buscar e instalar **Shadowsocks Connect**, el cliente oficial de Shadowsocks para Android.

***

### Sección B: Configurar Shadowsocks

***Paso 1***  

* Luego de instalar el cliente de Shadowsocks, **descarga el [archivo de configuración de Shadowsocks para Veles](https://explorer.veles.network/dapi/getShadowsocksConfig)**.  
[https://explorer.veles.network/dapi/getShadowsocksConfig](https://explorer.veles.network/dapi/getShadowsocksConfig)

***

***Paso 2***  

* Ejecuta el **cliente de Shadowsocks** y ve al menú **Importar perfil**.

***

***Paso 3***  

* Luego, completa el **"Hostname" (nombre de host)** con la **IP del Masternode** en la configuración de Shadowsocks.

***

***Paso 4***  

* **"Remote Port" (Puerto Remoto)** reemplazar con el Puerto Remoto de Veles **21344**

***

***Paso 5***  

* Cambiar **"Encryption Method" (Método de Encriptación)** a **aes-256-cfb**

***

***Paso 6***  

* Completar el **"Password"** con el password en la configuración de Shadowsocks.  

!!! cuidado "Advertencia"
    En la fase de testeo el password por defecto es - **`password`**  

***

### Sección C: Conectarse a la dVPN de Veles con Shadowsocks

***Paso 1***  

* Para conectarse, simplemente clickea el botón **Conectar**. Se solicitará que confirme que confía en la aplicación Shadowsocks. **Elige OK** para iniciar la conexión.  

!!! tip "User Tip"
 	Para **desconectarse** del cliente Shadowsocks, simplemente clickea **Desconectar**.  

***

### Sección D: Testear la conexión Shadowsocks 

***Paso 1***  

* Una vez que todo está instalado, es sencillo confirmar que todo está funcionando apropiadamente. Sin tener la conexión Shadowsocks activada, abra su navegador y vaya a [DNSLeakTest](https://www.dnsleaktest.com/).
El sitio le retornará la dirección IP asignada a usted por su proveedor de Internet, de la forma que el mundo lo ve. Para chequear su configuración de DNS a través del mismo sitio, clickee en Test Extendido y le informará que servidores DNS está utilizando.
Ahora, conecte su cliente Shadowsocks y refresque el navegador. La dirección IP totalmente nueva de su servidor VPN debería aparecer. Esto es como se muestra al mundo ahora. Nuevamente, el **Test Extendido** de  [DNSLeakTest](https://www.dnsleaktest.com/) chequeará su configuración de servidores DNS y le confirmará que está utilizando los resolvedores DNS de la dVPN Veles.

***

Si está todo correcto. felicitaciones! Has configurado la dVPN de Veles de manera exitosa. Si no es así, por favor contacta a soporte en [Discord](https://discord.gg/P528fGg) y ellos te asistirán.  

