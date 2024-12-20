<<<<<<< HEAD
# Extract Data for Further Analysis

## iOS Built-in Backup

* Windows: [https://support.apple.com/guide/itunes/itns3280/windows](https://support.apple.com/zh-tw/guide/itunes/itns3280/windows)
* macOS: [https://support.apple.com/guide/iphone/iph3ecf67d29/ios](https://support.apple.com/zh-tw/guide/iphone/iph3ecf67d29/ios)

## libimobiledevice

[libimobiledevice](http://www.libimobiledevice.org/) is a cross-platform software library that allows to interact with iOS devices. It can be used to perform a backup of the iPhone data, which may provide interesting data for a forensic analysis.

**Unlike other solutions presented in this guide, this backup will extract all the user data from the different applications and thus contains a lot of private information from the user (photos, messages etc.). Be mindful of what you do with it, and make sure the device owner consent to this extraction and to what is done with the data.**

### Install

libimobiledevice has packages for OpenSUSE, Fedora, Debian and Ubuntu Linux distributions, just do **apt install libimobiledevice** (or equivalent package manager).

On MAC OS, the easiest way is to install the [HomeBrew package manager](https://brew.sh/), and then install libimobiledevice with it with **brew install ideviceinstaller**

There is currently no easy way to install libimobiledevice on Windows, you will have to [manually compile it on your system](https://github.com/libimobiledevice/libimobiledevice/issues/582).

### Extract the Backup

Once libimobiledevice is installed, connect your iphone to your computer and accept the notification asking if your phone should trust the computer connected.

You can then check if the device is correctly connected with the computer with **idevice\_id -l** :
=======
# Extrair dados para análise adicional

## Backup no iOS

* Windows: [https://support.apple.com/pt-br/guide/itunes/itns3280/windows](https://support.apple.com/pt-br/guide/itunes/itns3280/windows)
* macOS: [https://support.apple.com/pt-br/guide/iphone/iph3ecf67d29/ios](https://support.apple.com/pt-br/guide/iphone/iph3ecf67d29/ios)

## libimobiledevice

A [libimobiledevice](http://www.libimobiledevice.org/) é uma biblioteca de software multiplataforma que permite interagir com dispositivos iOS. Ela pode ser usada para realizar um backup dos dados do iPhone, o que pode fornecer dados interessantes para uma análise forense.

**Ao contrário de outras soluções apresentadas neste guia, esse backup extrairá todos os dados do usuário dos diferentes aplicativos e, portanto, contém muitas informações privadas (fotos, mensagens etc.). Esteja atento ao que você fará com ele e certifique-se de que o proprietário do dispositivo consinta com essa extração e com o que será feito com os dados.**

### Instalação

O _libimobiledevice_ tem pacotes para as distribuições OpenSUSE, Fedora, Debian e Ubuntu Linux, basta fazer **apt install libimobiledevice** (ou gerenciador de pacotes equivalente).

No MacOS, a maneira mais fácil é instalar o [gerenciador de pacotes HomeBrew](https://brew.sh/) e, em seguida, instalar o libimobiledevice com ele com **brew install ideviceinstaller**

No momento, não há uma maneira fácil de instalar a libimobiledevice no Windows; você terá de [compilá-la manualmente em seu sistema](https://github.com/libimobiledevice/libimobiledevice/issues/582/).&#x20;

No momento, não há uma maneira fácil de instalar a libimobiledevice no Windows; você terá de [compilá-la manualmente em seu sistema](https://github.com/libimobiledevice/libimobiledevice/issues/582/).&#x20;

### Extrair o backup

Depois que a libimobiledevice estiver instalada, conecte o iPhone ao computador e aceite a notificação que pergunta se o telefone deve confiar no computador conectado.

Em seguida, você pode verificar se o dispositivo está conectado corretamente ao computador com **idevice\_id -l** :
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b

```
> idevice_id -l
6ff8a10037495eaf054018ed79fbf0e7e3c5bc2f
```

<<<<<<< HEAD
You can then do a backup of the system with the command **idevicebackup2 backup -d FOLDER**.

![backup process](../img/backup.png)

### Extract Data to a Readable Format

The data extracted by libimobile device are not in a readable format, to convert them into data as they are on the phone, you have to use another tool like [ideviceunback](https://github.com/inflex/ideviceunback).

First you need to download it and install it :
=======
Em seguida, você pode fazer um backup do sistema com o comando **idevicebackup2 backup -d FOLDER**.

![processo de backup](../.gitbook/assets/backup.png)

### Extrair dados em um formato legível

Os dados extraídos pelo libimobile device não estão em um formato legível; para convertê-los em dados como estão no telefone, é necessário usar outra ferramenta como o [ideviceunback](https://github.com/inflex/ideviceunback/).

Primeiro, você precisa fazer o download e instalá-la:
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b

```
$ git clone https://github.com/inflex/ideviceunback.git
$ make
```

<<<<<<< HEAD
You can now extract the files from the backup :
=======
Agora você pode extrair os arquivos do backup:
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b

```
./ideviceunback -v -i path/to/backup -o output/path
```
