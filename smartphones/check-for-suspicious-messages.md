<<<<<<< HEAD
# Check for Suspicious Messages

Messages containing links are a common attack vector.

![A message containing a link that infects the target with Cytrox Predator malware. Source: Citizen Lab](https://citizenlab.ca/wp-content/uploads/2021/12/Fig-7.png)

Links could be sent from any instant messaging apps or SMS. There are a few kinds of malicious links:

| Link target                                                             | Attacker goal                                                       | Sophistication | Mitigation                                      |
| ----------------------------------------------------------------------- | ------------------------------------------------------------------- | -------------- | ----------------------------------------------- |
| Phishing website, such as a webpage that looks like Google's login page | Trick user into entering personal data or passwords                 | Low            | Check webpage domain names and SSL certificates |
| App download                                                            | Convince user to download and install the app                       | Low            | Don't install apps outside of app stores        |
| Webpage containing web exploits, such as XSS (Cross Site Scripting)     | Steal online session cookies, or operate the currently open session | Medium         | Don't click on links sent by unknown people     |
| Webpage containing a browser exploit                                    | Exploit browser or app vulnerability                                | High           | Don't click on links sent by unknown people     |

### Saving messages

1. Copy the entire message including the link to clipboard
2. Alternatively, save a screenshot containing the full text
3. If you can, archive the link using the [Wayback Machine](https://web.archive.org/)

### Checking links

Simply Google search the link, or paste the link to sites like VirusTotal.
=======
# Verificar mensagens suspeitas

As mensagens que contêm links são um vetor de ataque comum.

<figure><img src="../.gitbook/assets/Captura de Tela 2024-12-11 às 22.18.08.jpg" alt="Uma mensagem contendo um link que infecta o alvo com o malware Cytrox Predator. "><figcaption><p>Uma mensagem contendo um link que infecta o alvo com o malware Cytrox Predator. Fonte: <a href="https://citizenlab.ca/wp-content/uploads/2021/12/Fig-7.png">Citizen Lab</a></p></figcaption></figure>

Os links podem ser enviados de qualquer aplicativo de mensagens instantâneas ou SMS. Há alguns tipos de links maliciosos:

| Alvo do Link                                                                              | Objetivo do Atacante                                                 | Sofisticação | Mitigação                                                      |
| ----------------------------------------------------------------------------------------- | -------------------------------------------------------------------- | ------------ | -------------------------------------------------------------- |
| Site de _phishing_, como uma página da web que se parece com a página de login do Google  | Enganar o usuário para que ele insira dados pessoais ou senhas       | Baixo        | Verificar nomes de domínio da página da web e certificados SSL |
| Download de aplicativo                                                                    | Convencer o usuário a fazer download e instalar o aplicativo         | Baixo        | Não instalar aplicativos fora das lojas de aplicativos         |
| Página da web contendo _exploits_ da web, como XSS (Cross Site Scripting)                 | Roubar cookies de sessão online ou operar a sessão aberta no momento | Média        | Não clicar em links enviados por pessoas desconhecidas         |
| Página da web que explora uma vulnerabilidade de um navegador.                            | Explorar a vulnerabilidade do navegador ou do aplicativo             | Alta         | Não clique em links enviados por pessoas desconhecidas         |

### Salvando mensagens

1. Copie a mensagem inteira, inclusive o link, para a área de transferência
2. Como alternativa, salve uma captura de tela contendo o texto completo
3. Se possível, arquive o link usando a [_Wayback Machine_](https://web.archive.org/).

### Verificação de links

Basta pesquisar o link no Google ou colar o link em sites como o [VirusTotal](https://www.virustotal.com).
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b
