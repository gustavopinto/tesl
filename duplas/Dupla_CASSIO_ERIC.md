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
Fizemos mais que isso e implementamos duas funções em um projeto na área de
processamento de linguagem natural (NLP, do inglês *natural language
processing*). O projeto converte números para sua versão por extenso em forma de
texto (e.g.: `68 -> "sessenta e oito"`), e tinha as funcionalidades de converter
números cardinais, ordinais e moedas (*currency*) com os métodos
`to_cardinal()`, `to_ordinal()` e `to_currency()`, respectivamente. Nós
implementamos os métodos `to_date()` (Cassio) e `to_time()` (Eric) para
converter de forma respectiva padrões de datas 
(e.g.: `12/5/1875 -> "doze de maio de mil, novecentos e setenta e cinco"`) e 
horas (e.g.: `14:55 -> "catorze e cinquenta e cinco"`).

Os métodos encontram-se dentro do arquivo
[lang_PT_BR.py](https://github.com/cassiobatista/num2words/blob/master/num2words/lang_PT_BR.py),
o qual encontra-se no repositório do 
[@cassiobatista](https://github.com/cassiobatista/num2words) que foi por sua vez
forked to repositório original do 
[@savoirfairelinux](https://github.com/savoirfairelinux/num2words).
