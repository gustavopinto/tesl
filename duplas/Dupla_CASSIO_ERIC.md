# Dupla CASSIO e ERIC

- Cassio Trindade Batista (cassio.batista.13@gmail.com, [@cassiobatista](https://github.com/cassiobatista))
- Eric Felipe de Oliveira Pereira (eric.cbcc@gmail.com, [@eriicf](https://github.com/eriicf))

## Link para atividades

- Atividade01: [link](https://docs.google.com/spreadsheets/d/1KE8YOIUFBwCTb0rkOSTE5cIdBi0Fqv2-fO4vAG79OeI/edit#gid=122497701) e [link](https://docs.google.com/spreadsheets/d/1fV-axR9_C6V3LBRMxadurJQAEyGZCzFRBiEPeVW-tUo/edit#gid=122497701)
- Atividade02: [link](https://docs.google.com/document/d/1ealVO6usU1eS3idCyYAy9e8tJCLbtb6hvh2gnyrpOnU/edit)

## Atividade 03
1. Experimentando comandos do `git`:    
    - `commit`: Serve para confirmar as mudanças feitas nos arquivos.    
    - `push`: Comando para enviar as mudanças salvas localmente para o repositório.    
    - `pull`: Comando para atualizar o repositório local com a mais nova versão.    
    - `checkout`: Comando para alternar entre os branch de um projeto.    
    - `log`: Comando para mostrar o id, autor, data e mensagens dos commits.    
    - `shortlog`: Mostra por usuário o número de commits.    

2. Imprimir saída de terminal similar:    
```
user@host ~/git-all/tesl (master) $ git shortlog -se
     1	AugustofCravo <49079453+AugustofCravo@users.noreply.github.com>
     4	Caio Shimada Rabello <xcaiosr@gmail.com>
     2	CaioMFRodrigues <caiomfrodrigues@gmail.com>
     2	Cassio Batista <cassio.batista.13@gmail.com>
     2	EdsonECS <49080256+EdsonECS@users.noreply.github.com>
     9	Filipe Saraiva <mail@filipesaraiva.info>
    18	Filipe Saraiva <saraiva@ufpa.br>
     2	Gabriel Quinto <gabrielquintoand@gmail.com>
    53	Gustavo Pinto <gustavohenrique.86@gmail.com>
     2	João Ferreira <lubien1996@gmail.com>
     2	Julio Cesar <julio.developer10@gmail.com>
     3	Lakshamana <guitrompa1@gmail.com>
     4	Lucas Gabriel de Souza <lucassouzaufpa@gmail.com>
     2	Lucas Monteiro <tavares.lucas1996@gmail.com>
     2	Lucas Souza <lucassouzaufpa@gmail.com>
     1	Ronaldd <ronaldppinho@gmail.com>
    11	Ronan Silva <contato.ronansilva@gmail.com>
     5	ThayssaRocha <49079381+ThayssaRocha@users.noreply.github.com>
     5	Uriel Campos <31864637+urielfcampos@users.noreply.github.com>
     2	VictorBSI <38796125+VictorBSI@users.noreply.github.com>
     1	Wagner Negrão <35495925+wagnerfns@users.noreply.github.com>
     1	eriicf <eric.cbcc@gmail.com>
     7	leojsv <49284606+leojsv@users.noreply.github.com>
     1	lubien <lubien1996@gmail.com>
     3	reinald28 <49073381+reinald28@users.noreply.github.com>
     2	tavareslucas <tavares.lucas1996@gmail.com>
```
Explicação do comando:     
```bash
git shortlog \
    -s # mostra somente o número de commits por autor, suprimindo qualquer outra descrição textual
    -e # mostra o email de cada autor
```      

3. Fazer um PR que melhore documentação/tradução de um projeto:     
    - Fizemos mais que isso e implementamos duas funções em um projeto na área
   de processamento de linguagem natural (NLP, do inglês *natural language
   processing*). O projeto converte números para sua versão por extenso em
   forma de texto (e.g.: `68 -> "sessenta e oito"`), e tinha as
   funcionalidades de converter números cardinais, ordinais e moedas
   (*currency*) com os métodos `to_cardinal()`, `to_ordinal()` e
   `to_currency()`, respectivamente. Nós implementamos os métodos `to_date()`
   (Cassio) e `to_time()` (Eric) para converter de forma respectiva padrões
   de datas (e.g.: `12/5/1875 -> "doze de maio de mil, oitocentos e setenta e
   cinco"`) e horas 
   (e.g.: `14:55 -> "catorze horas e cinquenta e cinco minutos"`).

    - O link para o projeto foi encontrado no site do
   [CodeTriage](https://www.codetriage.com/savoirfairelinux/num2words).

    - Os métodos encontram-se dentro do arquivo
   [lang_PT_BR.py](https://github.com/cassiobatista/num2words/blob/master/num2words/lang_PT_BR.py),
   o qual encontra-se no repositório do
   [@cassiobatista](https://github.com/cassiobatista/num2words) que foi por
   sua vez forked to repositório original do
   [@savoirfairelinux](https://github.com/savoirfairelinux/num2words). 

   - Por fim, o PR encontra-se neste 
   [link](https://github.com/savoirfairelinux/num2words/pull/250).

## Atividade 04
O projeto escolhido foi o
[num2words](https://github.com/savoirfairelinux/num2words) reportado na
atividade passada (03) cujo link foi encontrado no CodeTriage.

1. Selecione e identifique em um projeto:     
    - links para instalação: existe
   [aqui](https://github.com/savoirfairelinux/num2words#installation). Como o
   projeto é em Python, existe a opção de instalar pelo `pip` e pelo `setup.py`,
   mas a documentação para instalação local por desenvolvedores que desejam
   contribuir é escassa.      
    - documentação: simples para uso
   [aqui](https://github.com/savoirfairelinux/num2words#usage), porém quase
   nenhuma documentação sobre as classes e métodos é fornecida, nem por meio de
   comentários no código fonte     
    - documentação traduzida: não existe, apenas em inglês no próprio `README`.     
    - como contribuir: existe o arquivo
   [CONTRIBUTING](https://github.com/savoirfairelinux/num2words/blob/master/CONTRIBUTING.md)
   com um modelo para preenchimento de informações sobre as features adicionadas
   nos pull requests e com instruções para a formatação do código (PEP8).

2. Revise uma página e sumarize os problemas encontrados:    
    - A página indica a Wiki para procurar infos adicionais, mas na
   [Wiki](https://github.com/savoirfairelinux/num2words/wiki) só há informações
   para os idiomas Japonês, Finlandês e Telugo     
    - O software dá suporte a tradução de números em muitos idiomas, porém a
   documentação encontra-se apenas em inglês      
    - O repositório não possui nenhum arquivo LICENSE, apenas um arquivo
   [COPYING](https://github.com/savoirfairelinux/num2words/blob/master/COPYING),
   o que não é muito intuitivo para iniciantes.

3. Teste a documentação e sumarize os problemas encontrados     
    - falta documentação para instalação por partes dos desenvolvedores. A
   página indica apenas como instalar para usuários, usando `pip` e
   `setup.py`, mas não há indicações de configuração de variáveis de ambiente
   necessárias para executar o projeto localmente (sem permissão de admin),
   tampouco como fazer debug     
    - Na instalação pelo `pip` no Python3 Debian 9.8 Stretch, a função de 
   conversão de _currency_ não funciona para português brasileiro (e.g.: o 
   comportamento esperado seria `32.20 -> trinta e dois reais e vinte centavos`, 
   porém ocorre um erro dizendo que a opção não existe). Ou seja, o repositório
   disponível pelo pip ainda aponta para uma versão desatualizada.

## Atividade 05
1. Justifique o que acontece se um projeto de software não tiver nenhuma licença
definida.    
    - o projeto é tratado como se fosse privado, sendo **TODOS** os direitos de
   uso e redistribuição reservados exclusivamente ao autor do projeto
   (*copyright*).
2. Acesse o site choosealicense, e estude ao menos cinco licenças. Justifique
porque o site da disciplina tem a licença que tem.    
    - [GPLv3](https://choosealicense.com/licenses/gpl-3.0/): é considerada
    _strong copyleft_ por ser recíproca total, ou seja, todo e qualquer
    software derivado de um projeto sob esta licença deverá ser também
   redistribuído sob a mesma licença. 
    - [LGPLv3](https://choosealicense.com/licenses/lgpl-3.0/): criada com base
   na GPL original, a LGPL é considerada recíproca parcial. O `L` refere-se à
   "lesser", o que significa que a licença é mais permissiva por admitir que
   módulos possam ser copiados e redistribuídos sob diferentes licenças,
   incluindo as mais restritas que não disponibilizam código-fonte.
    - [Apache 2.0](https://choosealicense.com/licenses/apache-2.0/): é uma
   licença permissiva, que protege o autor no sentido de proibir forks de
   requerer patentes (direitos) sobre código eventualmente copiado e
   redistribuído. As notas de copyright do autor e a da licença Apache devem ser
   preservados (provavelmente no código), porém modificações e trabalhos maiores
   que tomem o projeto como base podem ser distribuídos em licenças diferentes e
   até mais restritas que não exijam distribuição do código-fonte.
    - [MIT](https://choosealicense.com/licenses/mit/): a licença MIT, conforme
   dito no blog [Exygy](https://exygy.com/which-license-should-i-use-mit-vs-apache-vs-gpl/),
   é uma licença permissiva que permite ao desenvolvedor "fazer o que quiser com
   o código", exigindo somente que o usuário mantenha as notas de copyright dos
   autores e da própria licença. Porém, a redistribuição podem ocorrer sob
   outras licenças, permitindo inclusive a não-divulgação dos códigos fontes, o
   que é de fundamental interesse para fins lucrativos (empresas, por exemplo).
    - [MPL 2.0](https://choosealicense.com/licenses/mpl-2.0/): a Mozilla Public
      License é uma licença recíproca parcial assim como a LGPL. O código fonte
   deve ser feito disponível e todos os arquivos, bem como suas eventuais
   modificações, devem ser disponibilizados sob a mesma licença. Porém, se o
   projeto forked for grande, é possível disponibilizá-lo sob uma diferente
   licença, incluindo as mais restritivas que não obrigam a compartilhar os
   fontes.
    - o site da disciplina possui licença *Creative Commons 4.0* pois não se
   trata de código de software propriamente dito. Conforme consta no
   [choosealicense.com](https://choosealicense.com/non-software/), "
   CC-BY-SA-4.0 is an open license used for non-software material ranging from
   datasets to videos." and "any open source software license or open license
   for media is applicable to software documentation."
3. Procure por projetos de software que utilize uma licença que não deveria ser
empregada em projetos de software.
    - https://gitlab.com/fb-nlp/nlp-generator
