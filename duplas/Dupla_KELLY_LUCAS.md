# Dupla KELLY e LUCAS
- Kelly do Socorro Silva da Costa (kellydosocorro@gmail.com, [@kellydosocorro](https://github.com/kellydosocorro))
- Lucas Gabriel de Souza (lucassouzaufpa@gmail.com, [@souzaluuk](https://github.com/souzaluuk))

## Link para atividades

- Atividade01: [link aqui](https://drive.google.com/drive/folders/1zPgeRZ-AI_rjgGjfCBBDnH7z3ksdkQtE?usp=sharing)

## Atividade 2
- Projeto escolhido: [Inkscape](https://gitlab.com/inkscape/inkscape)
- Identificar como os canais de comunicação das comunidades

  Os [canais de comunicação](https://inkscape.org/pt-br/comunidade/)
identificados foram:
    
  - Fórum [oficial](https://forum.inkscapecommunity.com/index.php) e fóruns 
regionais;
  - [Listas de 
e-mails](https://inkscape.org/community/mailing-lists/#inkscape-user);
  - [Chat](https://inkscape.org/community/discussion/);
  - [Galeria](https://inkscape.org/gallery/) com trabalhos de artistas que 
utilizam a ferramenta.

- Identificar como tarefas são sugeridas

  - Através de [Issues](https://gitlab.com/inkscape/inkscape/issues) que possuem 
estados (Open,Closed, e All) e 
[etiquetas](https://gitlab.com/inkscape/inkscape/labels) que associam o nível de 
importância, o estado em que a tarefa se encontra (exemplo: crash, building, 
blocker etc) e no que esta tarefa irá influenciar (exemplos: save+export, ui e 
text).

- Identificar como novas contribuições são avaliadas

  - No arquivo 
[CONTRIBUTING.md](https://gitlab.com/inkscape/inkscape/blob/master/CONTRIBUTING.md#contributing-to-inkscape) estão algumas informações sobre como os 
desenvolvedores podem contribuir para a ferramenta;

  - Nas solicitações de Merge: utilização de 
[Pipeline](https://gitlab.com/inkscape/inkscape/pipelines/) para testes, 
classificação destes erros por etiquetas e discussões em cima destas 
solicitações.

## Atividade 3
- Listando e descrevendo os seguintes comandos do `git`: `commit`, `push`, `pull`, `checkout`, `log` e `shortlog`.

  ```
  commit:
  Função: Registra as alterações no repositório
  Forma de utilização: git commit [opções]
  Exemplo de uso: git commit -m 'Aletaração na classe EXMEPLO'
  Onde o -m: Adiciona uma mensagem ao commit. Normalmente utilizada para indicar 
  sobre o que se trata aquela alteração.
  ```
  ```
  push:
  Função: Atualiza referências remotas junto aos objetos associados.
  Forma de utilização: git push [opções]
  Exemplo de uso: git push origin master
  Onde origin se refere ao repositório remoto de origem e master a branch master
  deste repositório remoto.
  ```
  ```
  pull:
  Função: Integra com outro repositório ou um branch local.
  Forma de utilização: git pull [opções]
  Exemplo de uso: git pull
  ```
  ```
  checkout:
  Função: alterna entre branches ou restaura arquivos da árvore de trabalho
  Forma de utilização: git checkout [opções]
  Exemplo de uso: git checkout branch-exemplo
  ```
  ```
  log:
  Função: exibe os logs de commit
  Forma de utilização: git log [opções]
  Exemplo de uso: git log --grep='Aletaração na classe EXMEPLO'
  ```
  ```
  shortlog:
  Função: resume a saída do 'git log'
  Forma de utilização: git shortlog [opções]
  Exemplo de uso: git shortlog -n -e -s
  ```
- O comando `git` que imprime uma saída neste formato `"quant_commits Autor <email>"` é:

  `git shortlog [-e|--email] [-s|--summary]`
  
  - Fazer um [pull-request](https://github.com/brython-dev/brython/pull/1094) que faça tradução de alguma parte da documentação de um projeto

## Atividade 4
- Selecione e identifique em um determinado projeto de software livre se a página inicial ou alguma página logo em seguida tem (ou não) links para instalação, documentação, documentação traduzida, e como contribuir. Coloque o projeto avaliado e os links encontrados (ou não);

  Projeto [Apache Tomcat](http://tomcat.apache.org/) ([GitHub](https://github.com/apache/tomcat))

  | Identificador | Site do Projeto | GitHub |
  |:------------- |:---------------:|:------:|
  | Instalação | [RUNNING.txt :-1:](https://tomcat.apache.org/tomcat-9.0-doc/RUNNING.txt) | [RUNNING.txt :+1:](https://github.com/apache/tomcat/blob/master/RUNNING.txt) |
  | Documentação | [:+1:](https://tomcat.apache.org/tomcat-9.0-doc/index.html) | [:-1:](http://localhost:8080/docs/) |
  | Documentação Traduzida | :open_hands: | :open_hands: |
  | Como contribuir | [Get Involved :+1:](https://tomcat.apache.org/getinvolved.html) | [CONTRIBUTING.md :+1:](https://github.com/apache/tomcat/blob/master/CONTRIBUTING.md) |

  > :-1: dificuldade na localização de informação e/ou falta adaptação do conteúdo para as diferentes fontes de informação (Site e GitHub)

  > :+1: facilidade de localização e coerência do conteúdo com a fonte de informação

  > :open_hands: nada encontrado

- Teste a documentação (por exemplo, siga as instruções de instalação) e sumarize os problemas encontrados;

- Revise uma página de um projeto de software livre e sumarize os problemas encontrados (o que falta para ela ser mais informativa).

Projeto [Video Maker](https://github.com/filipedeschamps/video-maker)
 
* Toda a informação de instalação é colocada diretamente no [README.md](https://github.com/filipedeschamps/video-maker/blob/master/README.md), o que acaba ele muito extenso. A sugestão seria criar uma pasta docs com a documentação específica para o usuário e atrelar ela a um link no read me;
* A descrição é muito básica, não é possível sondar com muita profundidade sobre o projeto;
* Não há nada indicando ou mesmo incitando a partipação de contribuidores para o projeto;
* Diante de tantas issue abertas, observou-se que não há um template estabelecido para estas (nem para pull requests).
