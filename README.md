# Parafuzo Resposta #

Contruir um jogo em linha de comando de pergunstas e respostas onde o jogador consegue responder apenas SIM ou NAO.
Essas perguntas devem estar em um arquivo yml e o sistema deve reconhecer variações e erros de digitação para respostas positivas e negativas.
Ao final das respostas deve ser exibido um total de respostas certas e erradas, as perguntas podem ser sequênciais ou aleatórias mas não devem se repetira a cada jogo.

Caso seja necessário algum procedimento antes de rodar os comandos, favor incluir um arquivo com as instruções.

Para entrega, enviar um Pull Request utilizando um fork ou um branch caso sua conta não permita repositórios privados.

## Avaliação ##

Será avaliado o bom funcionamento dos comandos e a arquitetura das classes.
Os testes devem cobrir o máximo possível dos casos.
Não é necessário criar o teste do arquivo executável basta focar nas classes internas.

## Comportamento ##

### Start ###

```
parafuzo-resposta
```
Deve exibir:
```
1. São Paulo é a melhor cidade para se viver no mundo?
> 
```

A cada resposta o sistema deve mostrar a próxima e só exibir algum tipo de resultado no final.
O usuário pode pular uma resposta simplesmente deixando ela em branco.

### Stop ###

Se o usuário responder todas as perguntas mostra o resultado e termina.
Se ele der um CTRL+C deve ser considerado como final do jogo e exibir o resultado também.

### Resultado ###

```
Você acertou 5 e errou 2 das 10 perguntas.
```

### Requisitos mínimos ###

* Validar sim, sin, Sim, SIM, si, não, nao, nau, Nao
