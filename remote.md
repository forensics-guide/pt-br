<<<<<<< HEAD
# Checking Devices Remotely

In this time of almost worldwide confinement, we are adding here a few steps that may help to check for potentially compromised devices remotely. It includes for now only solutions for Windows and Mac OS computers using [Teamviewer](https://www.teamviewer.com/en/) and [Chrome Remote Desktop](https://remotedesktop.google.com/), as we do not have yet any satisfying solution for smartphones (any suggestion [is welcome](https://github.com/securitywithoutborders/guide-to-quick-forensics/issues)).

## Limitations of Remote Forensic

### The Problem of Trust

With any remote desktop solution relying on a third party platform, there is an important question of trust. When you install such a remote desktop software, you have to know that the company developing the solution can use the software to access your computer but also can record any interaction you have through their solution. It is thus very important use a solution that you trust based on your threat model.

In this guide we use two software :

* [Teamviewer](https://www.teamviewer.com/en/) is a developed by TeamViewer AG, a German company based in Göppingen.
* [Chrome Remote Desktop](https://remotedesktop.google.com/) is developed by Google and is integrated in the Google ecosystem (which requires you to use Google accounts).

Teamviewer had several security issues in the past, the FireEye company claimed that it was breached by a [Chinese state-sponsored group in October 2019](https://www.securitynewspaper.com/2019/10/14/fireeye-confirms-that-apt14-group-hacked-teamviewer-attackers-would-have-accessed-billions-of-devices/). We tend to trust more Google for its security, but depending on your threat model, Teamviewer may be a better option. We are using Teamviewer for Windows here because Chrome Remote Desktop does not support well Mac OS yet (no file sharing).

### The Problem of Needing Online Access

Another issue with checking devices remotely is that you need the device to have access to Internet. As [explained before](safety.md), this can lead to some risks for the user. If the device is actually compromised and monitored remotely, the operators may identify that the user is receiving technical support and it may cause retaliation against the person you are trying to support.

You should make sure to address that risk before doing any remote support.

## Some Information on the Process

In order to schedule the check of a device remotely, you need to exchange beforehand with the person to let them know that :

* They will have to install a remote desktop software before
* They will have to stay in front of the computer during the check to enter the admin password (a check often last between 30 minutes and an hour)
* They will have to remove the remote desktop software after

Please keep in mind that [trust](trust.md) is a key part of any security support, so you should make sure that the process is clear for the person you are supporting and that they consent to it.

=======
# Verificação de dispositivos remotamente

Durante a época de confinamento em razão da pandemia COVID-19, adicionamos algumas etapas que podem ajudar a verificar remotamente os dispositivos potencialmente comprometidos. Por enquanto, elas incluem apenas soluções para computadores Windows e MacOS usando [Teamviewer](https://www.teamviewer.com/pt/?coupon=CMP-PR-BF24) e [Chrome Remote Desktop](https://remotedesktop.google.com/?pli=1\&hl=pt-BR), pois ainda não temos nenhuma solução satisfatória para smartphones.

## Limitações da perícia remota

### O problema da confiança

Em qualquer solução de área de trabalho remota que dependa de uma plataforma de terceiros, há uma questão importante de confiança. Quando você instala um software de acesso remoto desse tipo, precisa saber que a empresa que desenvolve a solução pode usar o software para acessar o seu computador, mas também pode gravar qualquer interação que você tenha por meio da solução. Portanto, é muito importante usar uma solução em que você confie, com base em seu modelo de ameaças.

Neste guia, usamos dois softwares:

* O [Teamviewer](https://www.teamviewer.com/pt/), desenvolvido pela TeamViewer AG, uma empresa alemã com sede em Göppingen.
* O [Chrome Remote Desktop](https://remotedesktop.google.com/?pli=1\&hl=pt-BR), desenvolvido pelo Google e integrado ao ecossistema do Google (o que exige o uso de contas do Google).

O Teamviewer teve vários problemas de segurança no passado, a empresa FireEye alegou que sofreu ataque de um [grupo patrocinado pelo Estado chinês em outubro de 2019](https://www.securitynewspaper.com/2019/10/14/fireeye-confirms-that-apt14-group-hacked-teamviewer-attackers-would-have-accessed-billions-of-devices/). Tendemos a confiar mais no Google por suas capacidades de segurança mas, dependendo do seu modelo de ameaças, o Teamviewer pode ser uma opção melhor. Estamos usando o Teamviewer para Windows, aqui, porque a Área de Trabalho Remota do Chrome ainda não é compatível com o MacOS (não permite compartilhamento de arquivos).

### O problema de precisar de acesso online

Outro problema com a verificação de dispositivos remotamente é que eles precisam de acesso à internet. Conforme explicado anteriormente, isso pode acarretar riscos para o usuário. Se o dispositivo estiver realmente comprometido e sendo monitorado remotamente, as operadores do monitoramento poderão identificar que o usuário está recebendo suporte técnico, o que poderá resultar em retaliação contra a pessoa a quem você está tentando apoiar.

Antes de prestar qualquer suporte remoto, você deve se certificar de abordar esse risco com a pessoa que está recebendo suporte.

## Algumas informações sobre o processo

Para executar a verificação de um dispositivo remotamente, é necessário conversar previamente com a pessoa para informá-la de que:

* Ela deverá instalar um software de área de trabalho remota antes
* Ela deverá permanecer na frente do computador durante a verificação para inserir a senha de administrador (uma verificação que geralmente dura de 30 minutos a uma hora)
* Ela deverá remover o software de área de trabalho remota depois

Lembre-se de que [confiança](trust.md) é uma parte fundamental de qualquer suporte de segurança, portanto, certifique-se de que o processo esteja claro para a pessoa que você está apoiando e que ela consinta com isso.
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b
