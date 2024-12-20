<<<<<<< HEAD
# Analyze Applications

## Scanner and antivirus apps

Some apps automatically check the apps installed on the system (to see if they are known to be malicious).

* [Koodous Antivirus](https://play.google.com/store/apps/details?id=com.koodous.android)
* [Lookout](https://play.google.com/store/apps/details?id=com.lookout)

These scanner apps work by extracting and uploading the APKs installed on the system to their own platform and comparing the APKs to known malwares. Some device information and potentially other personal information might be uploaded as well, one should check the platforms' privacy policy before installing and scanning with those apps.

Alternatively, there is an open-source antivirus application [Hypatia](https://github.com/Divested-Mobile/Hypatia), which utilizes signature databases from ClamAV, ESET and the [targeted threats list made by brotherder](https://github.com/botherder/targetedthreats).&#x20;

These scanner and antivirus apps can only see what other apps are installed, and cannot inspect deep into the operating system, because they themselves are sandboxed. However, medium to highly sophisticated malwares will embed themselves into the system without being shown as an app. These scanner and antivirus apps' knowledge of malwares also depends on their databases, whose sources often come from their enterprise customers. Thus, the scanner apps usually can only find malwares that package themselves as apps (which are usually medium to low sophistication), and are already known. However, these scanners can be installed and operated very easily, therefore they are still useful as a first-line test.

After finishing the check, uninstall the scanner apps to prevent further data collection.

## Extract Application Bundles (APKs)

Some tools require you to extract the APK files manually and upload them. Below are some tools that can extract APKs.

* [Apk Extractor](https://play.google.com/store/apps/details?id=com.ext.ui\&hl=zh\_TW)
* [Apk Extractor (open source, last update in 2018)](https://f-droid.org/packages/axp.tool.apkextractor/)
* [Kanade](https://github.com/alexrintt/kanade) (open source, last update in 2022)

Once an APK is extracted, one can also calculate its file hash (MD5 or SHA), and search for the hash using sites like VirusTotal.com .

## Online tools

### [Exodus Privacy](https://reports.exodus-privacy.eu.org/en/)

Exodus Privacy is a tool for privacy. It can analyze apps and list trackers contained in an app.

### [Hybrid-analysis.com](https://www.hybrid-analysis.com/)

Hybrid-analysis allows you to upload an APK file to scan. It checks the APK using various antivirus software and VirusTotal.

### [MobSF](https://github.com/MobSF/Mobile-Security-Framework-MobSF)

MobSF decompiles the application and analyze its contents, listing things like URLs, static files, and Activities. These can then be used to motivate further analysis.

There is a online version of MobSF available at [https://mobsf.live](https://mobsf.live).

You can also [host](https://mobsf.github.io/docs/#/installation) MobSF yourself, or use free hosting services like [Play with Docker](https://labs.play-with-docker.com/) to host a private MobSF instance. Play with Docker provides 4 hours of session time.

## Other tools

There are also other online analysis tools. The ones listed below are not specialized in APK.
=======
# Analisar aplicativos

## Aplicativos de verificação e antivírus

Alguns aplicativos verificam automaticamente os aplicativos instalados no sistema, para ver se eles são conhecidos como aplicações mal-intencionadas.

* [Koodous Antivirus ](https://play.google.com/store/apps/details?id=com.koodous.android)
* [Lookout](https://play.google.com/store/apps/details?id=com.lookout)

Recomendamos extremo cuidado se estiver considerando utilizar esses aplicativos de verificação, que funcionam extraindo e carregando os APKs instalados no sistema para sua própria plataforma, e comparando os APKs com malwares conhecidos. Informações do dispositivo e, provavelmente informações pessoais também podem ser enviadas para a plataforma. Verifique a política de privacidade das plataformas antes de instalar e fazer a varredura com esses aplicativos e faça uma avaliação de risco antes de utilizar estas plataformas.

Como alternativa, há um aplicativo antivírus de código aberto [Hypatia](https://github.com/Divested-Mobile/Hypatia), que utiliza bancos de dados de assinaturas do ClamAV, ESET e da [lista de ameaças direcionadas feita pelo brotherder](https://github.com/botherder/targetedthreats).

Esses aplicativos de scanner e antivírus só podem ver quais outros aplicativos estão instalados e não conseguem inspecionar profundamente o sistema operacional, pois eles próprios estão em _sandbox_. No entanto, malwares de média a alta sofisticação se incorporam ao sistema sem serem exibidos como um aplicativo. O conhecimento desses aplicativos de scanner e antivírus sobre malwares também depende de seus bancos de dados, cujas fontes geralmente vêm de seus clientes corporativos. Assim, os aplicativos de scanner geralmente só conseguem encontrar malwares que se empacotam como aplicativos (que geralmente são de média a baixa sofisticação) e que já são conhecidos. Entretanto, esses scanners podem ser instalados e operados com muita facilidade e, portanto, ainda são úteis como teste de primeira linha.

Após concluir a verificação, desinstale os aplicativos do scanner para evitar a coleta de dados adicionais.

### Extrair pacotes de aplicativos (APKs)

Algumas ferramentas exigem que você extraia os arquivos APK manualmente e os carregue. Abaixo estão algumas ferramentas que podem extrair APKs.

* [Apk Extractor](https://f-droid.org/packages/axp.tool.apkextractor/) (código aberto, última atualização em 2018)
* [Kanade](https://github.com/alexrintt/kanade) (código aberto, última atualização em 2022)
* [Androidqf](https://github.com/mvt-project/androidqf/) (Android Quick Forensics, Perícia Rápida do Android)

Depois que um APK é extraído, também é possível calcular o hash do arquivo (MD5 ou SHA) e pesquisar o hash usando sites como o VirusTotal.com .&#x20;

### Ferramentas online

### Exodus Privacy

O [Exodus Privacy](https://reports.exodus-privacy.eu.org/en/) é uma ferramenta para privacidade. Ele pode analisar aplicativos e listar rastreadores contidos em um aplicativo.

### Hybrid-analysis.com

O [Hybrid-analysis ](https://www.hybrid-analysis.com/)permite que você carregue um arquivo APK para análise. Ele verifica o APK usando vários softwares antivírus e o VirusTotal.

### MobSF

O [MobSF](https://github.com/MobSF/Mobile-Security-Framework-MobSF) descompila o aplicativo e analisa seu conteúdo, listando itens como URLs, arquivos estáticos e atividades. Esses itens podem ser usados para motivar outras análises.

Há uma versão on-line do MobSF disponível em [https://mobsf.live.](https://mobsf.live/)

Você também pode hospedar o MobSF por conta própria ou usar serviços de hospedagem gratuitos, como o Play with Docker, para hospedar uma instância privada do MobSF. O Play with Docker oferece 4 horas de tempo de sessão.&#x20;

Outras ferramentas

Há também outras ferramentas de análise online. As listadas abaixo não são especializadas em APK.
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b

* [https://cuckoo.cert.ee/](https://cuckoo.cert.ee/)
* [https://app.any.run/](https://app.any.run/)
* [https://www.virustotal.com/](https://www.virustotal.com/)

<<<<<<< HEAD
## Interpreting Analysis Results

The tools will produce a lot of technical information about the app, interpreting them would require technical understanding of how mobile apps work (such as: what are _content providers, services, activity_). However partial analysis could be achieved by simply checking if the files, URLs, IP addresses contained in the app is already known to be malicious.
=======
### Interpretação dos resultados da análise

As ferramentas produzirão muitas informações técnicas sobre o aplicativo. Para interpretá-las, seria necessário um conhecimento técnico de como os aplicativos móveis funcionam (por exemplo: o que são provedores de conteúdo, serviços, atividade). No entanto, uma análise parcial poderia ser feita simplesmente verificando se os arquivos, URLs e endereços IP contidos no aplicativo já são conhecidos como maliciosos.
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b
