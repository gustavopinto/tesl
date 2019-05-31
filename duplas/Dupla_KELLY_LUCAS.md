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

  - Informações para realização dos testes:
    - Projeto testado: [Apache Tomcat](https://github.com/apache/tomcat);
    - Documentações seguidas: [RUNNING.txt](https://github.com/apache/tomcat/blob/master/RUNNING.txt) e [Tomcat 9](https://tomcat.apache.org/tomcat-9.0-doc/);
    - SO: Manjaro Linux 18.0.4 64-bit.
  - Considerações:
    - As informações de instalação, configuração e execução do Software encontram-se no arquvivo RUNNING.txt;
    - No GitHub, tal informação é mais [direta](https://github.com/apache/tomcat#installation) e clara, diferentemente do site do projeto, em que deve-se ler atentamente a [documentação->introdução](http://tomcat.apache.org/tomcat-8.5-doc/introduction.html) até chegar na indicação para o arquvivo;
    - Considero que isso dificulta usuários que "cheguem" ao mesmo através do site e não pelo GitHub;
    - O arquivo RUNNING.txt por si só, é suficiente para a execução do Software, porém depende de documentações exeternas para pleno funcionamento;
    - A documentação "externa" a que se refere é do Java JRE, que é requisito para o funcionamento do Tomcat. Assim, a instalação do java não é orientada pelos mantenedores do projeto do Apache;
    - Fora isso, as orientações são bem claras e fáceis de realizar;
    - Por fim, as informações, apesar de claras, por vezes parecem mal organizadas ou dificies de encontrar, podendo ser uma barreira para novos contribuidores.

- Revise uma página de um projeto de software livre e sumarize os problemas encontrados (o que falta para ela ser mais informativa).
  
  Projeto [Video Maker](https://github.com/filipedeschamps/video-maker)
 
  * Toda a informação de instalação é colocada diretamente no [README.md](https://github.com/filipedeschamps/video-maker/blob/master/README.md), o que acaba ele muito extenso. A sugestão seria criar uma pasta docs com a documentação específica para o usuário e atrelar ela a um link no read me;
  * A descrição é muito básica, não é possível sondar com muita profundidade sobre o projeto;
  * Não há nada indicando ou mesmo incitando a partipação de contribuidores para o projeto;
  * Diante de tantas issue abertas, observou-se que não há um template estabelecido para estas (nem para pull requests).
  
## Atividade 5

- Justifique o que acontece se um projeto de software não tiver nenhuma licença definida.

  Se um software não definir uma licença para uso, automaticamente todos os direitos autorais são exclusivos de seu proprietário, logo, para alguém utilizar este código ele deve solicitar a autorização deste autor. Desta forma, um projeto deste tipo não poderá ser aceito em uma comunidade de software livre, para isto, ele deve adquirir uma licença que o permita ser considerado como um.

- Acesse o site [choosealicense](https://choosealicense.com/), e estude ao menos cinco licenças. Justifique porque o site da disciplina tem a licença que tem.

  - [APACHE LICENSE 2.0](https://choosealicense.com/licenses/apache-2.0/): Esta é uma licença permissiva utilizada para comunidades e autoriza o uso comercial, distribuição, modificação, patente e uso pessoal sob a condição de apresentar cópias desta e do copyright junto ao software, bem como a documentação de mudanças no software.
 
  - [MIT License](https://choosealicense.com/licenses/mit/): Esta licença é permissiva, de forma a permitir o uso comercial, distribuição, modificação e uso privado sob a condição de que uma cópia desta e do copyright sejam disponibilizadas junto ao software.
 
  - [GNU General Public License v2.0](https://choosealicense.com/licenses/gpl-2.0/): Esta licença permite o uso comercial, a distribuição, a modificaão e o uso privado mediante a disponibilidade do software após sua distribuição, uma cópia da licença e do copyright deve ir junto do software, as modificações neste devem estar sob a mesma licença (ou similar em alguns casos) do código original bem como a documentação das mudanças realizadas no código.
 
  - [ISC License](https://choosealicense.com/licenses/isc/): É uma licença permissiva que garante a comercialização, distribuição, modificação e uso privado sob a única condição de que a licença e o copyright estejam inclusos com o código.
 
  - [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/): Esta licença permite o uso comercial, a distribuição, a modificaão, a patente (sua principal diferença em relação à GNU General Public License v2.0) e o uso privado mediante a disponibilidade do software após sua distribuição, uma cópia da licença e do copyright deve ir junto do software, as modificações neste devem estar sob a mesma licença (ou similar em alguns casos) do código original bem como a documentação das mudanças realizadas no código.
 
  A licença usada pelo site da disciplina é a Creative Commons Attribution 4.0 International Public License que permite a cópia e redistribuição de materiais bem como sua adaptação para qualquer propósito, incluso uso comercial, de tal forma que estes direitos não podem ser revogados enquanto aqueles que fazem uso destes materiais cumprirem os termos de licença.

- Procure por projetos de software que utilize uma licença que não deveria ser empregada em projetos de software.

  O software [Dspace](https://github.com/DSpace/DSpace/blob/master/LICENSE) que utiliza uma licença Copyright mesmo sendo um software livre.

## Atividade 6

- Selecione 5 projetos de software livre famosos (pelo menos 1000 estrelas) e coloque os links para seus respectivos site, repositório de código fonte, bug tracking e ferramentas de comunicação.
  - Kubernetes:
    - [Site](https://kubernetes.io);
    - [Repositório](https://github.com/kubernetes/);
    - [Código fonte](https://github.com/kubernetes/kubernetes);
    - [Bug Tracking](https://github.com/kubernetes/kubernetes/issues);
    - Comunicação: [Repositório da comunidade](), [Fórum](https://discuss.kubernetes.io/), [Twitter](https://twitter.com/kubernetesio), [Stackoverflow](https://stackoverflow.com/search?q=kubernetes) e [Slack](http://slack.k8s.io/).
  - QGIS:
    - [Site]();
    - [Repositório](https://github.com/qgis);
    - [Código fonte](https://github.com/qgis/QGIS);
    - Bug tracking: [Aplicações](https://issues.qgis.org/projects/qgis/issues), [Website](https://github.com/qgis/QGIS-Website/issues), [Documentação](https://github.com/qgis/QGIS-Documentation/issues) e via [Readmine](https://issues.qgis.org/projects/qgis/issues);
    - Comunicação: [Lista de e-mails](https://qgis.org/en/site/getinvolved/mailinglists.html#qgis-mailinglists), [Twitter](http://twitter.com/qgis) e [Facebook](https://www.facebook.com/pages/QGIS-Quantum-GIS-/298112000235096).
  - Symfony:
    - [Site](https://symfony.com);
    - [Repositório](https://github.com/symfony/);
    - [Código fonte](https://github.com/symfony/symfony);
    - [Bug tracking](https://github.com/symfony/symfony/issues);
    - Comunicação: [Twitter](https://twitter.com/symfony), [Facebook](https://www.facebook.com/SymfonyFramework/), [Stackoverflow](https://stackoverflow.com/questions/tagged/symfony), [Slack](https://symfony.com/slack), [Mensagem direta](https://symfony.com/support).
  - Deno:
    - [Site](https://deno.land);
    - [Repositório](https://github.com/denoland/);
    - [Código fonte](https://github.com/denoland/deno);
    - [Bug tracking](https://github.com/denoland/deno/issues);
    - Comunicação: [Chat](https://gitter.im/denolife/Lobby). 
  - Home Assistant:
    - [Site](https://www.home-assistant.io/);
    - [Repositório](https://github.com/home-assistant/);
    - [Código fonte](https://github.com/home-assistant/home-assistant);
    - [Bug tracking](https://github.com/home-assistant/home-assistant/issues);
    - Comunicação: [Fóruns](https://community.home-assistant.io/), [Chat](https://www.home-assistant.io/join-chat/), [Facebook](https://facebook.com/homeassistantio) e [Twitter](https://twitter.com/home_assistant).

- Encontre 3 exemplos de pedidos de feature ou resolução de bugs que foram implementadas, coloque o link para elas e faça um relatório crítico sobre o fluxo: era bug ou feature? foi iniciado por um usuário ou desenvolvedor? os desenvolvedores foram reticentes ou abertos para a descrição realizada? houve pedido de mais informações? foi resolvido rapidamente ou demorou? houve algum impecilho técnico ou social para essa resolução? quem resolveu o problema foi um desenvolvedor experiente, novato ou algum usuário?
  - [vuetify](https://github.com/vuetifyjs/vuetify/issues/7223): A issue em questão se trata de uma Feature Request feita por um usuário que foi rapidamente atendida, porém, "etiquetada" como uma duplicata. O membro do repositório que atendeu rapidamente relacionou o pedido à [outra issue](https://github.com/vuetifyjs/vuetify/issues/2961) já existente e igualmente fechada. É importante observar que certamente o template pronto para bugs e features contribui para o atendimento rápido neste repositório.
 
  - [gatsby](https://github.com/gatsbyjs/gatsby/issues/14075): A issue em questão era uma dúvida que não foi respondida sendo encerrada pela própria pessoa que a adicionou apenas 2 horas depois de sua publicação.
 
  - [angular](https://github.com/angular/angular/issues/30500): A issue em questão foi um bug report que não foi bem explicitada pelo usuário que a publicou, sendo encerrada sem uma solução por um dos membros do repositório.

- Encontre e discuta formas de priorizar requisitos em projetos de software livre.
  
  Uma das possíveis formas de se levar em consideração seria através de uma classificação, ocorrendo de tal forma:
 
  - Manter uma equipe responsável por lidar com estes requisitos atenta aos mais diversos meios de comunidação e feature requests;
  - Verificar se é uma issue ou uma sugestão de equipe/comunidade. Priorizar sugestões de equipe/comunidade e categorizar com labels cada issue adicionada;
  - Verificar a pertinência, a relevância e o impacto destas junto aos membros chaves do repositório;
  - Estimar o esforço em implementação deste requisito;
  - Dispensar mais esforço naqueles que parecem mais agradar à comunidade;
  - E com base na análise anterior, decidir os requisitos a serem mantidos e deixa-los claros à comunidade informando sua respectiva importância, impacto e status(se não iniciado, em andamento e concluído ambos bem detalhados).


## Atividade 7
- Explique o são Linters e qual a sua importância?

  O linter é uma ferramenta que tem por objetivo analisar códigos-fontes afim de localizar e sinalizar potênciais erros de padrão de codificação e indentação. Sua importância reside no fato de auxiliar na garantia de padrônização de códigos dos projetos, principalmente em trabalhos colaborativos.
  
- Indique um guia de boas práticas de codificação em linguagem de programação (exceto: Python, PHP e Java)

  Guia de boas práticas para codificação de projetos JavaScript do Google: [Google JavaScritp Style Guide](https://google.github.io/styleguide/jsguide.html)

- Indique um guia de boas práticas de codificação em frameworks de linguagem de programação.

  Guia de boas práticas do [Jquery](https://contribute.jquery.org/style-guide/), um framework de Javascript.

## Atividade 8
- Explique que o são métodos ágeis e qual a sua importância no processo de desenvolvimento de softwares?

  Métodos ágeis são um conjunto de abordagens alternativas para gerência de projetos nas quais são definidas iterações curtas cujos resultados são medidos através da conclusão do produto. Os métodos ágeis são importantes para o desenvolvimento de software devido ao fato de sua simplicidade e eficácia na gerências das atividades que compõe em projeto bem como nas interações dos membros da equipe. 

- Procure um projeto e indique um commit que indique trabalho feito em par, ou seja, um commit que tenha multiplos autores.
  
  Commit feito no repositório do [Angular](https://github.com/angular/angular/commit/deb77bd3df2300eb8ed46f5015e730afd8dc5c78).

- Procure um projeto que utilize kanban e coloque o link para a utilização desse método.

  Repositório do projeto [GNOME](https://gitlab.gnome.org/groups/GNOME/-/boards).
  
## Atividade 9

- Por que utilizar testes unitários?

  Os testes unitários são importantes pois visam realizar o teste da menor parte possível de um código (por exemplo, teste de uma função/método) de forma a manter a mínima coerência possível dada modificações realizadas naquele método/função.

- Quais vantagens de utilizar integração contínua?

  - Redução do trabalho manual durante o processo de integração;
  - Melhor entendimento da equipe sobre o trabalho de seus colegas;
  - Redução dos erros e reposta mais rápida dado o surgimento de um;
  - Disponibilização do software em ciclos menores;
  - Diminuição no tempo de lançamento de atualização de produtos.
