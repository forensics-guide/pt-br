<<<<<<< HEAD
# Introduction
=======
# Introdução
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b

Muitas vezes, membros da sociedade civil têm a suspeita, mais ou menos justificada, de estarem sendo vigiados. Talvez eles tenham tido anomalias em seus computadores ou dispositivos móveis, ou tenham motivos para acreditar que algumas de suas comunicações tenham sido interceptadas.

<<<<<<< HEAD
Technologists and first responders working in civil society are often requested assistance with the inspection of human rights defenders' devices. The purpose of this guide is to provide an introduction to a methodology that could be useful for the quick assessment of potential infections.
=======
Tecnólogas e socorristas que trabalham na sociedade civil são frequentemente solicitados a ajudar na inspeção de dispositivos de defensoras dos direitos humanos. O objetivo deste guia é apresentar uma introdução a uma metodologia que pode ser útil para a avaliação rápida de possíveis infecções.
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b

Embora a metodologia apresentada aqui não seja, de forma alguma, suficiente para fornecer uma avaliação definitiva e conclusiva sobre a limpeza de um dispositivo suspeito, ela pode ajudar, pelo menos, a identificar as infecções mais óbvias. Em última análise, cabe à sua intuição, e à compreensão do contexto, determinar quais são as melhores recomendações a serem dadas. Esperamos que este guia o ajude a começar a fazer a Análise Forense Rápida e lhe forneça as ferramentas e técnicas para desenvolver suas habilidades.

<<<<<<< HEAD
**Note**:

* This guide is a fork from the [original guide by Security Without Borders](https://github.com/securitywithoutborders/guide-to-quick-forensics).
* This fork aims to keep existing content up-to-date, while adding latest information.
* This fork is currently under development. You can contribute to this text [here](https://github.com/pellaeon/guide-to-quick-forensics).

## Why do Quick Forensics?

Learning to perform quick forensics helps determine whether additional resources might be required or not.

Learning to triage helps determine whether the case requires additional resources or not. Being able to extract relevant data means that in-depth investigators will not need access to the device (at least, not immediately). More people doing triaging, means better scalability of incident response in civil society. Researchers working on targeted threats against civil society are few, and mostly focused on publications.
=======
#### Observação

* Este guia é uma bifurcação _(fork_) de [guia original do Security without Borders](https://github.com/securitywithoutborders/guide-to-quick-forensics)
* Essa bifurcação tem como objetivo manter o conteúdo existente atualizado e adicionar as informações mais recentes.
* Esta bifurcação está em desenvolvimento no momento. Você pode contribuir com a versão em inglês  [aqui](https://github.com/pellaeon/guide-to-quick-forensics) e com a [**versão em português aqui**](https://github.com/celsobessa/guide-to-quick-forensics/tree/pt-br).

### Por que fazer Análises Forenses Rápidas?
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b

Aprender a executar uma análise forense rápida ajuda a determinar se recursos adicionais podem ser necessários ou não.

Aprender a fazer triagem ajuda a determinar se o caso requer recursos adicionais. A capacidade de extrair dados relevantes significa que as investigadoras que vão mais a fundo não precisarão acessar o dispositivo (pelo menos não imediatamente). Quanto mais pessoas fizerem triagens, melhor será a escalabilidade da resposta a incidentes na sociedade civil. As pesquisadoras que trabalham com ameaças direcionadas à sociedade civil são poucas e se concentram principalmente em publicações.

### Os objetivos

Ao executar uma análise forense rápida e responder a um comprometimento potencial, temos os seguintes objetivos gerais:

1. Tentar determinar se o dispositivo está realmente potencialmente infectado.
2. Extrair dados suficientes para verificação subsequente e que possam ser úteis para investigação posterior (por exemplo, para determinar que tipo de malware infectou o dispositivo).
3. Determinar o que fazer com o dispositivo e como ajudar ainda mais seu proprietário.
