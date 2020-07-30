# Dividindo o documento em arquivos

Para documentos grandes, é interessante poder separar o texto em diversos arquivos.
Dessa forma temos uma organização melhor do nosso texto.

## Arquivo principal

O arquivo principal será aquele que organizará todo o texto.
Esse arquivo terá o preâmbulo do documento e o ambiente `document` dentro dele.

Dentro do ambiente principal, se quisermos inserir um arquivo `texto.tex`, iremos usar o comando

``` tex
\input{caminho/para/texto}
```

Como no exemplo, o uso da extensão `.tex` no nome do arquivo não é obrigatório.

### Exemplo

O documento que foi criado na [seção 2](./hello_world.md) foi divido em arquivos.
Nele, cada seção do texto ficou em um arquivo separado. No arquivo principal, o código ficou:

``` tex
% Preâmbulo omitido

\begin{document}

    \maketitle
    \tableofcontents

    \input{introducao}
    \input{método}
    \input{resultado}
    \input{conclusao}

\end{document}
```

## Arquivos secundários

Os arquivos `.tex` que cotém o texto não precisam de nenhum comando para funcionarem. Qualquer biblioteca necessária para o arquivo **deverá ser importada no arquivo principal**.