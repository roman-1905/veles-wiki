Name:               Guía Linux de Veles en OpenVPN
Image:              images/download/android.png
GuideType:          Guía de usuario
OS:                 Android
VelesdApp:          dVPN
Protocol:           OpenVPN
Requirements:       cliente OpenVPN
Difficulty:         Muy fácil
EstimatedTime:      3 minutos


# Guía de OpenVPN para Android
Esto te guiará a través del proceso de instalar y utilizar OpenVPN en la plataforma Android.  

Si requiere más ayuda por favor contacte a nuestro equipo de soporte @ [Discord](https://discord.gg/P528fGg)

## Requerimientos
1) **Instalar el cliente OpenVPN**  
2) **Descargar la configuración de OpenVPN de Veles**  

## Contenido
* **Sección A**: Descargar e instalar OpenVPN
* **Sección B**: Configurar OpenVPN
* **Sección C**: Conectarse a la dVPN de Veles
* **Sección D**: Testear la conexión VPN 
***

### Sección A: Descargar e instalar OpenVPN

***Paso 1***

* Abrir **Google Play Store**. Buscar e instalar **Android OpenVPN Connect**, el cliente oficial de OpenVPN para Android.

***

### Sección B: Configurar OpenVPN

***Paso 1***  

* Luego de instalar OpenVPN, **descarga el [archivo de configuración de OpenVPN para Veles](https://explorer.veles.network/dapi/getOpenVPNConfig)**.  
[https://explorer.veles.network/dapi/getOpenVPNConfig](https://explorer.veles.network/dapi/getOpenVPNConfig)

***

***Paso 2***  

* Ejecuta la **app OpenVPN** y ve al menú **Importar perfil**.

***

***Paso 3***  

* **Luego navega a la ubicación donde se ha descargado el archivo de perfil y selecciónalo**. La app tomará nota de que un perfil ha sido importado.

***

### Sección C: Conectarse a la dVPN de Veles

***Paso 1***  

* Para conectarse, simplemente clickea el botón **Conectar**. Se solicitará que confirme que confía en la aplicación OpenVPN. **Elige OK** para iniciar la conexión.  

!!! tip "User Tip"
 	Para **desconectarse de la VPN**, vuelve a la app OpenVPN y clickea **Desconectar**.  

***

### Sección D: Testear la conexión VPN 

***Paso 1***  

* Una vez que todo está instalado, es sencillo confirmar que todo está funcionando apropiadamente. Sin tener la conexión VPN activada, abra su navegador y vaya a [DNSLeakTest](https://www.dnsleaktest.com/).
El sitio le retornará la dirección IP asignada a usted por su proveedor de Internet, de la forma que el mundo lo ve. Para chequear su configuración de DNS a través del mismo sitio, clickee en Test Extendido y le informará que servidores DNS está utilizando.
Ahora, conecte su cliente VPN y refresque el navegador. La dirección IP totalmente nueva de su servidor VPN debería aparecer. Esto es como se muestra al mundo ahora. Nuevamente, el **Test Extendido** de  [DNSLeakTest](https://www.dnsleaktest.com/) chequeará su configuración de servidores DNS y le confirmará que está utilizando los resolvedores DNS de la dVPN Veles.

***

Si está todo correcto. felicitaciones! Has configurado la dVPN de Veles de manera exitosa. Si no es así, por favor contacta a soporte en [Discord](https://discord.gg/P528fGg) y ellos te asistirán.  
