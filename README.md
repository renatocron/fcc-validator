# fcc-validator

Verificador de arquivos **ATSEFCC** (`.FCC`) — Financiamento Coletivo de Campanha do TSE.

**Use aqui:** https://renatocron.github.io/fcc-validator/

Solte um arquivo `.FCC` na página. O navegador processa o arquivo localmente. A página não envia o arquivo para nenhum servidor.

O verificador confere cada campo de cada registro (HEADER, DETALHE 1, DETALHE 2 e TRAILER) contra o layout v3.0 (07/2022):

- posição, tamanho, tipo e valor fixo de cada campo;
- regras de preenchimento (zeros à esquerda, espaços à direita ou à esquerda);
- datas na máscara DDMMAAAA;
- códigos permitidos de espécie do recurso e de meio de pagamento;
- dígitos verificadores de CPF e de CNPJ;
- ordem dos registros, tamanho de linha (375 caracteres), terminadores de linha e quebra de linha final;
- nomenclatura do arquivo;
- totais cruzados: contagem do TRAILER, total de doações individuais, soma dos valores e crédito = total − taxa.

Fonte do layout: TSE — *Especificação de Layout de Arquivo, Financiamento Coletivo de Campanha*, versão 3.0, de 2022-07-04, reeditada em julho de 2026 para o sistema Conta+JE.
