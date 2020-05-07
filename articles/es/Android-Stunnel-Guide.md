Name:               Guía Linux de Veles en Stunnel
Image:              images/download/android.png
GuideType:          Guía de usuario
OS:                 Android
VelesdApp:          dVPN
Protocol:           TLS/SSL (stunnel), OpenVPN
Requirements:       Cliente de Stunnel para Veles, cliente OpenVPN
Difficulty:         Moderado
EstimatedTime:      7 minutos

# Guía de Stunnel para Android
Esto te guiará a través del proceso de instalar y utilizar Stunnel en la plataforma Android.  

Si requiere más ayuda por favor contacte a nuestro equipo de soporte @ [Discord](https://discord.gg/P528fGg)

## Requirimientos
1) **Tener instalado [[Guía de OpenVPN para Android]]**  
2) **Instalar Stunnel para Veles**   
3) **Descargar la configuración de Shielded OpenVPN para Veles**  

## Contenido
* **Sección A**: Descargar e instalar Veles Stunnel
* **Sección B**: Configurar Veles Stunnel
* **Sección C**: Conectarse a la dVPN de Veles con Veles Stunnel
* **Sección D**: Testear la conexión VPN 
***

### Sección A: Descargar e instalar Veles Stunnel

***Paso 1***

* Abrir **Google Play Store**. Buscar e instalar **Veles Stunnel**, el cliente oficial de Stunnel sobre Veles para Android.

***

### Sección B: Configurar Veles Stunnel

***Paso 1***  

* Luego de instalar Veles Stunnel, **descarga el [archivo de configuración de Stunnel para Veles](https://explorer.veles.network/dapi/getShieldedOpenVPNConfig)**.  
[https://explorer.veles.network/dapi/getShieldedOpenVPNConfig](https://explorer.veles.network/dapi/getShieldedOpenVPNConfig)

***

***Paso 2***  

* Ejecuta la **app OpenVPN** y ve al menú **Importar perfil**.

***

***Paso 3***  

* **Luego navega a la ubicación donde se ha descargado el archivo de perfil y selecciónalo**. La app tomará nota de que un perfil ha sido importado.

***

***Paso 4***  

* **Inicia la app de Veles Stunnel** y clickea en el menú para **Configurar**.

***

***Paso 5***  

* Reemplazar **"MasternodeIP"** con la IP del masternode al que va a conectarse.  

!!! tip "User Tip"
	Puede chequear la IP  en la app de OpenVPN Connect cuando importa el perfil shielded-veles.ovpn  

***

### Sección C: Conectarse a la dVPN de Veles con Veles Stunnel

***Paso 1***  

* Ahora, inicie Veles Stunnel. Abra la app y **presione el botón de la página de Inicio**.

!!! tip "User Tip"
	**Para desconectarse** de Veles Stunnel, simplemente presione el botón en la página de Inicio nuevamente.  

***

***Paso 2***  

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
