# Acer Aspire A515-52G-Hackintosh-Sonoma 14.5

## Funcionando...
 - [x] Áudio, microfone e headphone jack
 - [x] GPU Intel
 - [x] Gerenciamento de Energia
 - [x] Brilho
 - [x] Ethernet
 - [x] Bluetooth
 - [x] Touchpad + Teclado
 - [x] WebCam
 - [x] Usb
 - [x] Leitor de cartão de Memória


 ## Não funciona
 - [x] Nvidia GTX, não possui suporte

## Não testado
 - [x] HDMI
 - [x] Wifi Intel, necessário trocar por uma placa compatível
 
## Instalação
 
 ### BIOS
* *Main* → Network Boot → **Disable**
* *Main* → Wake on LAN → **Disable**
* *Main* → Touchpad → **Basic**
* *Main* → Lid Open Resume → **Enable**
* *Main* → Wake on USB while lid closed → **Disable**
* *Main* → D2D Recovery → **Disable**
* *Main* → Fast boot → **Disable**
* *Advanced* → Intel VTX → **Disable**
* *Advanced* → Intel VID → **Disable**
* *Security* → Set Supervisor Password → Coloque uma senha para poder desativar o Secure Boot.
* *Boot* → Boot Mode → **UEFI**
* *Boot* → Secure Boot → **Disable**

### Indicações:

- Download IMG: https://www.olarila.com/forum/
- Criar Instalador: https://hackintoshbrasil.com/forum/topic/7-como-criar-o-instalador/
- Instalar sem usar essa EFI, alterar a EFI após instalação

### Pré instalação:

### Pós instalação

- Desabilitar Hibernation : Não é suportado e pode causar problemas.

```sh

$ sudo pmset -a hibernatemode 0

$ sudo rm /var/vm/sleepimage

$ sudo mkdir /var/vm/sleepimage

$ sudo pmset -a standby 0

$ sudo pmset -a autopoweroff 0

- Caso esteja utilizando SSD. Habilitar TRIM

$sudo trimforce enable

```

---

