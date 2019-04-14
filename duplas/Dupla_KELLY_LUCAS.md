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
  
