<<<<<<< HEAD
# Check Storage

Instead of checking every file on the storage, there are a few shortcuts to check for suspicious files:

1. Download history of the user-preferred browser
2. "Recently used" section in the file manager

## Search for APK Files

Sometimes users are tricked into downloading and installing APK files and the APK files were left in phone storage. By searching for APK files, we might find APK files that were installed in the past.

## Search for Suspicious Files

Less sophisticated malware might leave a trace on the phone by writing files in the internal storage (or SD card).

Look for these kinds of files, and search their path in Google:

* `.log`, `.txt` files: might be log files created by malware or spyware
* Files containing copies or backup of sensitive user information, such as call logs, chat history, or contact lists. These information are usually kept only in app storage (storage area only accessible to an app), unless the user intentionally exports them. So any unintentional exports might be a sign of malware stealing data or apps malfunctioning. These files should be deleted quickly after use because the internal storage is less protected.
* `.so` files: `so` stands for "shared object", which can be understood as an extension to an executable file. Existence of `.so` files might indicate that they were loaded and executed.
=======
# Verificar armazenamento

Em vez de verificar todos os arquivos no armazenamento, existem alguns atalhos para verificar se há arquivos suspeitos:

1. Histórico de downloads do navegador preferido do usuário
2. Seção "Usado recentemente" no gerenciador de arquivos

## Pesquisar arquivos APK

Às vezes, os usuários são enganados para baixar e instalar arquivos APK e eles foram deixados no armazenamento do telefone. Ao pesquisar por arquivos APK, é possível que encontremos alguns que foram instalados no passado.

## Pesquisar por arquivos suspeitos

Malware menos sofisticado pode deixar um rastro no telefone gravando arquivos no armazenamento interno (ou cartão SD).

Procure esses tipos de arquivos e pesquise seu caminho no Google:

* Arquivos `.log`, `.txt`: podem ser arquivos de log criados por malware ou spyware
* Arquivos contendo cópias ou backup de informações confidenciais do usuário, como registros de chamadas, histórico de bate-papo ou listas de contatos. Essas informações geralmente são mantidas apenas no armazenamento do aplicativo (área de armazenamento acessível apenas a um aplicativo), a menos que o usuário as exporte intencionalmente. Portanto, qualquer exportação não intencional pode ser um sinal de malware roubando dados, ou de aplicativos com defeito. Esses arquivos devem ser excluídos rapidamente após o uso porque o armazenamento interno é menos protegido.
* Arquivos `.so`: `so` significa "objeto compartilhado", que pode ser entendido (_shared object_) como uma extensão de um arquivo executável. A existência de arquivos `.so` pode indicar que eles foram carregados e executados.
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b
