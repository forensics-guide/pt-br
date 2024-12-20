<<<<<<< HEAD
# Smartphone System Architecture

Smartphones are basically small handheld computers, the major architectural distinction from computers are:

* Systems being more locked down:
  * Non-customizable bootloaders
* Addition of special purpose co-processors
  * Secure enclave
  * Baseband
  * Image-processing
  * AI acceleration

### Co-processors

Co-processors are processors used only for a particular purpose other than the system. The co-processors helps the main _application processor_ to handle certain tasks, thus have to communicate with it. Co-processors often run their own embedded operating system and application and could not be directly controlled by the user. Co-processors often has privileged access to system resources and user data, so they are sometimes targets of more sophisticated exploitations. Due to the locked-down nature, it is difficult to audit or obtain forensic data from co-processors. For the purpose of this guide, you will only need to know that:

* Co-processors can be exploited
* Co-processor exploits are sophisticated and uncommon

The rest of this guide will thus focus on the softwares running on the application processor.

### Operating System

Smartphone operating systems differ from computer operating systems in that they implement more controls and isolation between different system components and applications, so that a compromised component could not easily affect the whole system.

![](https://developer.android.com/guide/platform/images/android-stack\_2x.png)

It is possible for attackers to exploit kernel vulnerabilities, however these vulnerabilities are quite rare and usually requires sophisticated techniques to exploit.

### System Applications

System applications may contain vulnerabilities. Once exploited, they can cause greater harm than exploiting user applications, because they usually have more privilege to change the underlying system. One common example is the built-in browser, which is often exploited.

### User Applications

User applications are least privileged. However, if the permissions are granted, they can access sensitive user information, so they can still cause great harm. They can also sometimes trick or exploit the underlying system to gain more control.
=======
# Arquitetura do sistema do smartphone

Os smartphones são basicamente pequenos computadores de mão, e as principais diferenças arquitetônicas em relação aos computadores são:

* Os sistemas são mais protegidos:
  * Carregadores de inicialização (_bootloaders_) não são customizáveis
* Adição de coprocessadores para fins especiais
  * Enclave seguro
  * Banda base (_Baseband_, para telefonia)
  * Processamento de imagens
  * Aceleradores de IA

### Coprocessadores

Os coprocessadores são processadores usados somente para uma finalidade específica que não seja o sistema. Eles ajudam o processador principal a lidar com determinadas tarefas e, portanto, precisam se comunicar com ele. Os coprocessadores geralmente executam seu próprio sistema operacional e aplicativo incorporados, e não podem ser controlados diretamente pelo usuário. Geralmente, eles têm acesso privilegiado aos recursos do sistema e aos dados do usuário, portanto, às vezes, são alvos de ataques de _exploit_ mais sofisticadas. Devido à sua natureza protegida, é difícil auditar ou obter dados forenses dos coprocessadores. Para os fins deste guia, você só precisa saber que:

* Os coprocessadores podem ser atacados por _exploits_
* Os ataques de _exploits_ a coprocessadores são sofisticados e incomuns

O restante deste guia se concentrará, portanto, nos softwares executados no processador do aplicativo.

### Sistema operacional

Os sistemas operacionais dos smartphones diferem dos sistemas operacionais dos computadores, pois implementam mais controles e isolamento entre os diferentes componentes e aplicativos do sistema, de modo que um componente comprometido não possa afetar facilmente todo o sistema.

![](../.gitbook/assets/android-stack_2x-pt-br.png)

É possível que os invasores explorem as vulnerabilidades do [núcleo](https://pt.wikipedia.org/wiki/N%C3%BAcleo_\(sistema_operacional\)) (_kernel),_ mas essas vulnerabilidades são bastante raras e geralmente exigem técnicas sofisticadas para serem exploradas.

### Aplicativos do sistema

Os aplicativos do sistema podem conter vulnerabilidades. Uma vez atacados, eles podem causar mais danos do que a exploração de aplicativos de usuário, pois geralmente têm mais privilégios para alterar o sistema subjacente. Um exemplo comum é o navegador incorporado, que é violado com frequência.

### Aplicativos de usuário

Os aplicativos de usuário são menos privilegiados. No entanto, se as permissões forem concedidas, eles podem acessar informações confidenciais do usuário e causar grandes danos. Às vezes, eles também podem enganar ou explorar o sistema subjacente para obter mais controle.
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b
