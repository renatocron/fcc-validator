# fcc-validator

Client-side validator for TSE SPCE **ATSEFCC** (`.FCC`) crowdfunding donation files (Financiamento Coletivo de Campanha).

**Use it:** https://renatocron.github.io/fcc-validator/

Drop a `.FCC` file on the page. Nothing is uploaded — all parsing and validation happens in your browser.

Checks every field of every record (HEADER, DETALHE 1, DETALHE 2, TRAILER) against the layout spec v3.0 (07/2022): positions, sizes, types, fixed values, padding/alignment rules, DDMMAAAA dates, allowed payment codes, CPF/CNPJ check digits, record order, line length (375), line endings, trailing line break, filename convention, and cross-record totals (trailer count, doações individuais, soma dos valores, crédito = total − taxa).

Layout source: TSE — *Especificação de Layout de Arquivo, SPCE Financiamento Coletivo*, versão 3.0 (04/07/2022).
