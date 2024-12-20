<<<<<<< HEAD
# Extract Data for Further Analysis

[pcqf](https://github.com/botherder/pcqf) is a tool that allows to dump startup information and actual processes, along with memory for further analysis. It is really helpful for instance if you do not have time to check for everything on the computer and want to double check if there is anything suspicious later on.

You should run this program from a USB key with enough storage space, double click on the binary file and follow the instructions.

![pcqf](../.gitbook/assets/pcqf1.PNG)

Unless you have a good reason to do so, it is recommended not to take a memory snapshot as it is contains a lot of private information (it may contains passwords for instance).

Once finished, it will create a folder named by the acquisition ID (a sequence of hexadecimal number) , which contains :

* A `profile.json` file containing basic information on the computer system.
* A `process_list.json` file containing a list of running processes.
* An `autoruns.json` file containing a list of all items with persistence on the system.
* An `autoruns_bins/` folder containing copies of the files and executables marked for persistence in the previous JSON file.
* An `process_bins/` folder containing copies of running processes.
* If requested, a `memory/` folder will contain a physical memory dump as well as some metadata.
=======
# Extrair dados para análise adicional

O [pcqf](https://github.com/botherder/pcqf) é uma ferramenta que permite fazer uma descarga (_dump_) das informações de inicialização e processos reais, juntamente com a memória para análise posterior. Ela é realmente útil, por exemplo, se você não tiver tempo para verificar tudo no computador e quiser verificar novamente se há algo suspeito mais tarde. Você deve executar esse programa a partir de uma chave USB com espaço de armazenamento suficiente, clicar duas vezes no arquivo binário e seguir as instruções.

![pcqf](../.gitbook/assets/pcqf1.PNG)

A menos que você tenha um bom motivo para fazer isso, é recomendável não tirar um instantâneo da memória, pois ele contém muitas informações privadas (pode conter senhas, por exemplo).

Uma vez concluído, ele criará uma pasta nomeada pelo ID da aquisição (uma sequência de números hexadecimais), que contém:

* Um arquivo `profile.json` que contém informações básicas sobre o sistema do computador.
* Um arquivo `process_list.json` que contém uma lista de processos em execução.
* Um arquivo `autoruns.json` que contém uma lista de todos os itens com persistência no sistema.
* Uma pasta `autoruns_bins/` que contém cópias dos arquivos e executáveis marcados para persistência no arquivo JSON anterior.
* Uma pasta `process_bins/` que contém cópias dos processos em execução.
* Se solicitado, uma pasta `memory/` conterá um despejo de memória física, bem como alguns metadados.
>>>>>>> 08764f159532245dbd422df65bec951b7323b37b
