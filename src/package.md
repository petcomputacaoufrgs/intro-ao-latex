# \usepackage

Logo após a configuração da classe, podemos importar pacotes que auxiliem na elaboração do documento usando o comando `\usepackage[parâmetros]{pacote}`.

Existem milhares de pacotes no LaTeX, cada um com suas especificações e opções.
Vamos trazer aqui alguns pacotes que acreditamos serem os mais essenciais para o primeiro documento, porém você pode encontrar diversos outros pacotes na internet[^1].

- `\usepackage[encode]{inputenc}`:
    Por padrão, o LaTeX usa o encode ASCII, que não possuí acentos, cedilhas, entre outros. O pacote **inputenc** permite que você escolha outro encode para contornar esse problema. No overleaf ele coloca automaticamente o encode utf8, mas também podemos usar o encode latin-1;
- `\usepackage[language]{babel}`:
    Organiza o documento de acordo com as regras de pontuação e lingua de um país. Para usar as regras do Brasil, basta passar a opção brazil para o pacote;
- `\usepackage{indentfirst}`:
    Esse pacote cria o espaçamento de parágrafo automaticamente após iniciar uma nova linha. Não precisa de parâmetros.
- `\usepackage{amsmath}`[^2]:
    Insere inúmeras opções e comandos para o ambiente matemático.
- `\usepackage{graphicx}`[^2]:
    Utilizamos esse pacote quando precisamos importar imagens para o documento.
- `\usepackage{ragged2e}`[^2]:
    Esse pacote insere o alinhamento justificado ao texto.


[^1]: [CTAN - lista de pacotes com documentação](https://ctan.org/pkg)

[^2]: Esses pacotes serão vistos em um outro momento de forma mais detalhada.

### Exemplo

Utilizando o exemplo anterior, podemos configurar o nosso documento para escrever o nosso documento em português:

``` tex
\documentclass[a4paper, 12pt, twocolumn, notitlepage]{article}

\usepackage[utf8]{inputenc}
\usepackage[brazil]{babel}
\usepackage{indentfirst}
```