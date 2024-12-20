# MVT

<<<<<<< HEAD
[Mobile Verification Toolkit (MVT)](https://github.com/mvt-project/mvt) is a collection of utilities to simplify and automate the process of gathering forensic traces helpful to identify a potential compromise of Android and iOS devices.

On Android, MVT works mainly by collecting system information using [ADB](https://developer.android.com/studio/command-line/adb).

## Install
=======
O [Kit de Verificação de Aparelhos Móveis (MVT, _Mobile Verification Toolkit_)](https://github.com/mvt-project/mvt) é uma coleção de utilitários para simplificar e automatizar o processo de coleta de rastros forenses úteis para identificar um possível comprometimento de dispositivos Android e iOS, como telefones e tablets.

No Android, o MVT funciona principalmente coletando informações do sistema usando o [ADB (Android Debug Bridge).](https://developer.android.com/tools/adb?hl=pt-br)

## Instalar
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b

```
pip3 install mvt
```

<<<<<<< HEAD
## Running Check

`mvt-android check-adb --output <directory>`

## Looking for Indicators in MVT Output

In this section, we will explain the types of data gathered by MVT on Android and what indicators to look for.

### command.log

`command.log` is the main MVT output. Pay attention on the `WARNING` messages. Many of MVT's automated checks overlaps with the manual checks introduced in [android.md](../android.md "mention"). Such as:
=======
## Executando verificação

`mvt-android check-adb --output <diretório>`

## Procurando indicadores na saída do MVT

Nesta seção, explicaremos os tipos de dados coletados pelo MVT no Android e quais indicadores procurar.

### command.log

`command.log` é a saída principal do MVT. Preste atenção nas mensagens `WARNING`. Muitas das verificações automatizadas do MVT se sobrepõem às verificações manuais introduzidas em [android.md](../android.md "mention"). Como:
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b

```
WARNING - Found suspicious setting "package_verifier_user_consent = -1" (disabled Google Play Protect)
```

<<<<<<< HEAD
Also, pay attention to "_Found non-system package with name..._", which lists the packages not installed from the Google Play Store.

```
INFO - Found non-system package with name "tech.httptoolkit.android.v1"       installed by "None" on 2022-06-11 12:36:40
```

In the above example, a HTTPS interception tool used for debugging is installed by "None" because it was installed manually by opening a APK file in a file browser.

When encountering a suspicious app, check the file path and hash in `packages.json`:

```
    {    
        "package_name": "tech.httptoolkit.android.v1",
        "file_name": "/data/app/tech.httptoolkit.android.v1-M3BLlBPO_DgoSTQ4yZWWDw==/base.apk",
        "installer": null,
        "disabled": false,
        "system": false,
        "third_party": true,
        "files": [
            {
                "path": "/data/app/tech.httptoolkit.android.v1-M3BLlBPO_DgoSTQ4yZWWDw==/base.apk",
                "md5": "081dd91d110072491e8312c8f5fd8b0b",
                "sha1": "067057b7e6f95d7bd4fefeceb77f9133eec23c50",
                "sha256": "85c551370465b289eaa90ee293a3cf212cf1fc7aa6a74fca220b0283680689e7",
                "sha512":                                                                                                                  "bc906a2d674f4827a262773b33d51493805f22271105a34e346d307397742f9f51a81be8edfe70ea08a1aa04be6effda9cdd08b67a13f7cb02aab89514a7bb34"
            }
        ],
        "uid": "10142",
        "version_name": "1.3.2",
        "version_code": "22 minSdk=21 targetSdk=29",
        "timestamp": "2022-06-11 12:36:40",
        "first_install_time": "2022-06-11 12:36:42",
        "last_update_time": "2022-06-11 12:36:42",
        "requested_permissions": [
            "android.permission.INTERNET",
            "android.permission.ACCESS_NETWORK_STATE",
            "android.permission.FOREGROUND_SERVICE",
            "android.permission.CAMERA",
            "android.permission.WAKE_LOCK",
            "com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE",
            "android.permission.READ_EXTERNAL_STORAGE"
        ]
    },
```

Search the package name or file hash on VirusTotal or Koodous platform and read the analysis.

### packages.json

As [noted](https://nex.sx/tech/2022/01/28/a-primer-on-android-forensics.html) by MVT's developer:

> Walking through this `packages.json` file is an important first step. Prioritize looking at non-system and third-party apps. Look out for any that were disabled (for example, a commercial security app marked as disabled might be a red flag). Search online for package names and hashes of those apps that do not look familiar, have odd names, or might show an unusual _installer_.

### files/

In the output folder, there is a `files/`folder, which contains files pulled from `/data/local/tmp` on the phone. This path is often used as a staging area for malwares.

Check the file hashes of those files on VirusTotal.

### Other indicators

{% embed url="https://nex.sx/tech/2022/01/28/a-primer-on-android-forensics.html" %}

{% embed url="https://nex.sx/tech/2022/02/04/diving-deeper-in-android-system-diagnostics.html" %}
=======
Além disso, preste atenção em "_Found non-system package with name..._", que lista os pacotes não instalados da Google Play Store.

```
INFO - Found non-system package with name "tech.httptoolkit.android.v1" installed by "None" on 2022-06-11 12:36:40
```

No exemplo acima, uma ferramenta de interceptação HTTPS usada para depuração foi instalada por "None" porque foi instalada manualmente abrindo um arquivo APK em um navegador de arquivos.

Ao encontrar um aplicativo suspeito, verifique o caminho do arquivo e o hash em `packages.json`:

```
{
"package_name": "tech.httptoolkit.android.v1",
"file_name": "/data/app/tech.httptoolkit.android.v1-M3BLlBPO_DgoSTQ4yZWWDw==/base.apk",
"installer": null,
"disabled": false,
"system": false,
"third_party": true,
"files": [
{
"path": "/data/app/tech.httptoolkit.android.v1-M3BLlBPO_DgoSTQ4yZWWDw==/base.apk",
"md5": "081dd91d110072491e8312c8f5fd8b0b",
"sha1": "067057b7e6f95d7bd4fefeceb77f9133eec23c50", "sha256": "85c551370465b289eaa90ee293a3cf212cf1fc7aa6a74fca220b0283680689e7", "sha512": f4827a262773b33d51493805f22271105a34e346d307397742f9f51a81be8edfe70ea08a1aa04be6effda9cdd08b67a13f7cb02aab89514a7bb34" } ], "uid": "10142",
"version_name": "1.3.2",
"version_code": "22 minSdk=21 targetSdk=29",
"timestamp": "2022-06-11 12:36:40",
"first_install_time": "2022-06-11 12:36:42",
"last_update_time": "2022-06-11 12:36:42",
"requested_permissions": [
"android.permission.INTERNET",
"android.permission.ACCESS_NETWORK_STATE",
"android.permission.FOREGROUND_SERVICE",
"android.permission.CAMERA",
"android.permission.WAKE_LOCK",
"com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE",
"android.permission.READ_EXTERNAL_STORAGE"
]
},
```

Pesquise o nome do pacote ou hash do arquivo na plataforma VirusTotal ou Koodous e leia a análise.

### packages.json

Conforme [observado](https://web.archive.org/web/20230506002932/https://nex.sx/blog/2022/01/28/a-primer-on-android-forensics.html) pelo desenvolvedor do MVT:

> Percorrer este arquivo `packages.json` é um primeiro passo importante. Priorize a análise de aplicativos que não sejam do sistema e de terceiros. Fique atento a qualquer um que tenha sido desabilitado (por exemplo, um aplicativo de segurança comercial marcado como desabilitado pode ser um sinal de alerta). Pesquise na internet nomes de pacotes e hashes desses aplicativos que não pareçam familiares, tenham nomes estranhos ou possam mostrar um _instalador_ incomum.

### files/

Na pasta de saída, há uma pasta `files/`, que contém arquivos extraídos de `/data/local/tmp` no telefone. Esse caminho é frequentemente usado como uma área de preparação para malwares.

Verifique os hashes desses arquivos no VirusTotal.

### Outros indicadores

* A Primer on Android Forensics (Uma Introdução à Perícia em Android), de Nex. . Versão arrquivada em [https://web.archive.org/web/20230506002932/https://nex.sx/blog/2022/01/28/a-primer-on-android-forensics.html](https://web.archive.org/web/20230506002932/https://nex.sx/blog/2022/01/28/a-primer-on-android-forensics.html)
* Diving Deeper in Android System Diagnostics and Remote Forensics (Indo Mais Fundo no Diagnóstico de Sistema e Perícia Remota em Android), de Nex. Versão arquivada em [https://web.archive.org/web/20220928085050/https://nex.sx/tech/2022/02/04/diving-deeper-in-android-system-diagnostics.html](https://web.archive.org/web/20220928085050/https://nex.sx/tech/2022/02/04/diving-deeper-in-android-system-diagnostics.html)
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b
