<<<<<<< HEAD
# Review XProtect Logs

[XProtect](https://book.hacktricks.xyz/macos-hardening/macos-security-and-privilege-escalation/macos-security-protections/macos-gatekeeper#xprotect) is a built-in **anti-malware** feature in macOS. XProtect **checks any application when it's first launched or modified against its database** of known malware and unsafe file types. When you download a file through certain apps, such as Safari, Mail, or Messages, XProtect automatically scans the file. If it matches any known malware in its database, XProtect will **prevent the file from running** and alert you to the threat.

For background system scanning, macOS previously used MRT. Since 2022, a new module [XProtect Remediator](https://eclecticlight.co/2023/06/12/malware-detection-and-remediation-by-xprotect-remediator/) was added to macOS.

To check the scan results of XProtect Remediator, use [XProCheck](https://eclecticlight.co/2022/09/05/xprocheck-a-new-utility-to-inspect-anti-malware-scans/). However, Apple has not published details about Remediator, so the logs may be hard to understand.
=======
# Revisar logs do XProtect

O [XProtect](https://book.hacktricks.xyz/macos-hardening/macos-security-and-privilege-escalation/macos-security-protections/macos-gatekeeper#xprotect/) é um recurso **anti-malware** incorporado ao macOS. O XProtect **verifica qualquer aplicativo quando ele é iniciado ou modificado pela primeira vez em seu banco de dados** de malware conhecido e tipos de arquivos não seguros. Quando você faz download de um arquivo por meio de determinados aplicativos, como Safari, Mail ou Messages, o XProtect verifica automaticamente o arquivo. Se ele corresponder a algum malware conhecido em seu banco de dados, o XProtect **impedirá a execução do arquivo** e o alertará sobre a ameaça.

Para a varredura do sistema em segundo plano, o macOS usava anteriormente o MRT. Desde 2022, um novo módulo [XProtect Remediator](https://book.hacktricks.xyz/macos-hardening/macos-security-and-privilege-escalation/macos-security-protections/macos-gatekeeper#xprotect/) foi adicionado ao macOS.

Para verificar os resultados da verificação do XProtect Remediator, use o [XProCheck](https://eclecticlight.co/2022/09/05/xprocheck-a-new-utility-to-inspect-anti-malware-scans/). No entanto, a Apple não publicou detalhes sobre o Remediator, portanto, os registros podem ser difíceis de entender.
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b
