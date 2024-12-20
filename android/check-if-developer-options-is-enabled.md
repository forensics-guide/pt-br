<<<<<<< HEAD
# Check if Developer Options is Enabled

If USB Debugging in [Developer Options](https://developer.android.com/studio/debug/dev-options) is enabled, one can control a phone using the Android Debug Bridge (ADB) over USB, or over Wifi if Wifi Debugging is enabled. ADB would also allow attackers to drop executables onto the phone in `/data/local/tmp` and execute it as the `shell` system user.

Unless the phone under check is being used for Android App development, **it is not normal for USB Debugging to be enabled.** You should find out the reason why and when the user enabled it.

If USB Debugging is enabled, you should:

* Check whether there are apps installed via ADB, and if so, analyze these apps.
* Check for suspicious files under `/data/local/tmp`

Once you have determined that no malware was installed using ADB, USB Debugging should be disabled.

For high risk users, checking the two items above is not sufficient, since there are many other ways ADB could be used to infect a device, and it might also be possible that after the infection the attacker cleared out their traces. Thus, we recommend factory wiping the device before continue using it.
=======
# Verificar se as opções do desenvolvedor estão ativadas

Se a Depuração USB em [Opções do Desenvolvedor](https://developer.android.com/studio/debug/dev-options) estiver habilitada, é possível controlar um telefone usando o Android Debug Bridge (ADB) via USB ou via WiFi, se a Depuração WiFi estiver habilitada. O ADB também pode permitir que invasores coloquem executáveis ​​no telefone em `/data/local/tmp` e o executem como usuário do sistema `shell`.

A menos que o telefone sob verificação esteja sendo usado para desenvolvimento de aplicativos Android, **não é normal que a Depuração USB esteja habilitada.** Você deve descobrir o motivo e quando o usuário a habilitou.

Se a Depuração USB estiver habilitada, você deve:

* Verificar se há aplicativos instalados via ADB e, em caso positivo, analisar esses aplicativos.
* Verificar se há arquivos suspeitos em `/data/local/tmp`

Depois de determinar que nenhum malware foi instalado usando o ADB, a Depuração USB deve ser desabilitada.

Para usuários de alto risco, verificar os dois itens acima não é suficiente, pois há muitas outras maneiras pelas quais o ADB pode ser usado para infectar um dispositivo, e também pode ser possível que, após a infecção, o invasor tenha apagado seus rastros. Portanto, recomendamos limpar o dispositivo de fábrica antes de continuar a usá-lo.
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b
