# Metodologia

<<<<<<< HEAD
The methodology for doing quick forensics can be quite ad-hoc, and eventually with time you will develop your own. This guide should help in this process. Generally, when trying to triage a possible infection, you will look for any anomaly that you are able to identify on the device. Such anomalies, for example, can be:

1. Applications and processes running on the device that you and the owner of the device do not recognize. Applications and processes that show some unusual characteristics, such as suspicious names and file locations, or attempts at hiding.
2. Because spyware normally would want to be able to survive a shutdown of the device, you will look for applications which maintain persistence over the device and are therefore registered for automatic execution at startup.
3. Suspicious network connections to infrastructure and services that you and the owner of the device do not recognize.
4. Accounts, profiles or configurations that do not belong to the device owner.

While it is not possible to compile an exhaustive checklist of precise anomalies to look out for, the process of developing a robust quick forensics methodology will require *training your eye*, by inspecting as many devices as you can get your hands on. Eventually, you will start recognizing patterns across various operating systems, and become more rapid and efficient at discarding legitimate applications and spotting those that stand out. It takes practice.

**Warning**: the methodology we describe in this guide heavily relies on using tools that are publicly available and highly popular. Because of this, more sophisticated malware might be capable of bypassing or evading these tools and trick you into believing you are looking at a clean system. Therefore, **this methodology needs to be considered a best effort.** You have to take into account the possibility of false negatives and adjust your assessment accordingly (particularly in relation to the device owner's [safety](safety.md)).

## Considerations on legal litigation

Under some circumstances, it is possible that the owner of the device has an interest in pursuing some legal action against the perpetrators of the attack you are documenting, or perhaps the producers of the technology used to conduct it. This could be the case, for example, with victims of domestic abuse, or perhaps with activists seeking to prove some illegal surveillance of their communications.

If you believe the person you are assisting might be interested in any form of legal litigation, especially based on your work, you might need to adapt your methodology. From country to country, from jurisdiction to jurisdiction, rules and best practices for gathering digital evidence admissible in court can vary. Generally, because of [chain of custody](https://en.wikipedia.org/wiki/Chain_of_custody) and to safeguard the integrity of the device, data acquisition (especially from phones) might be heavily restricted.

You should inform yourself about the laws and the standard practices from the jurisdiction you normally operate in. Ideally, you should seek advise from local forensics specialists and maybe even seek the assistance of an accredited forensics firm.
=======
A metodologia para realizar análises forenses rápidas pode ser bastante [ad-hoc](https://pt.wikipedia.org/wiki/Ad_hoc) e com o tempo você desenvolverá a sua própria metodologia. Este guia deve ajudar nesse processo. Em geral, ao tentar fazer a triagem de uma possível infecção, você procurará qualquer anomalia que possa identificar no dispositivo. Essas anomalias, por exemplo, podem ser:

1. Aplicativos e processos em execução no dispositivo que você e a proprietária do dispositivo não reconhecem. Aplicativos e processos que apresentam algumas características incomuns, como nomes e locais de arquivos suspeitos ou tentativas de ocultação.
2. Como o _spyware_ normalmente deseja sobreviver a um desligamento do dispositivo, você procurará aplicativos que busquem ter persistência no dispositivo e, portanto, estejam registrados para abrirem/executarem de forma automática na inicialização.
3. Conexões de rede suspeitas com infraestrutura e serviços que você e a proprietária do dispositivo não reconhecem.
4. Contas, perfis ou configurações que não pertencem à proprietária do dispositivo.

Embora não seja possível compilar uma lista de verificação exaustiva de anomalias precisas a serem observadas, o processo de desenvolvimento de uma metodologia forense rápida e robusta exigirá _treinar o seu olhar_, inspecionando o maior número de dispositivos possível. Eventualmente, você começará a reconhecer padrões em vários sistemas operacionais e se tornará mais rápida e eficiente para descartar aplicativos legítimos e identificar aqueles que se destacam. Isso requer prática.

**Atenção**: a metodologia que descrevemos neste guia depende muito do uso de ferramentas que estão disponíveis publicamente e são altamente populares. Por esse motivo, _malwares_ mais sofisticados podem ser capazes de enganar ou evadir-se dessas ferramentas e levar você a acreditar que está vendo um sistema limpo. Portanto, **essa metodologia precisa ser considerada o melhor esforço possível.** Você deve levar em conta a possibilidade de falsos negativos e ajustar sua avaliação de acordo com isso (especialmente em relação à [segurança](safety.md) da proprietária do dispositivo).

## Considerações sobre processos legais

Em algumas circunstâncias, é possível que a proprietária do dispositivo tenha interesse em entrar com uma ação legal contra os autores do ataque que você está documentando ou, talvez, contra os produtores da tecnologia usada para o ataque. Esse pode ser o caso, por exemplo, de vítimas de violência doméstica ou talvez de ativistas que buscam provar a vigilância ilegal de suas comunicações.

Se você acredita que a pessoa que está ajudando pode estar interessada em qualquer forma de litígio judicial, especialmente com base no seu trabalho, talvez seja necessário adaptar sua metodologia. As regras e as práticas recomendadas para a coleta de evidências digitais admissíveis em um tribunal podem variar de país para país, e de jurisdição para jurisdição. Geralmente, para proteger a integridade do dispositivo e garantir a [cadeia de custódia](https://pt.wikipedia.org/wiki/Cadeia_de_cust%C3%B3dia), a aquisição de dados (especialmente de telefones) pode ser muito restrita.

Você deve se informar sobre as leis e as práticas padrão da jurisdição em que normalmente opera. Idealmente, você deve buscar orientação de especialistas forenses locais e talvez até mesmo buscar a assistência de uma empresa forense credenciada.
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b
