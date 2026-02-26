### Registro 0000 – Identificação da empresa

| Campo                     | Nº Campo | Tipo      | Casas/Decimais | Formato | Valor | Comentário                                      |
|---------------------------|----------|-----------|----------------|---------|-------|-------------------------------------------------|
| Identificação do registro | 1        | Caractere |                |         | 0000  | Fixo 0000 – Identificação do registro           |
| Inscrição da empresa      | 2        | Caractere |                |         |       | CNPJ/CPF/CEI/CAEPF da empresa. Informar apenas números. |

---

### Registro 0200 – Contas contábeis

| Campo                          | Nº Campo | Tipo      | Formato     | Valor | Comentário |
|--------------------------------|----------|-----------|-------------|-------|------------|
| Identificação do registro      | 1        | Caractere |             | 0200  | Fixo 0200 – Identificação do Registro. |
| Código reduzido                | 2        | Numérico  |             |       | |
| Classificação contábil         | 3        | Caractere |             |       | |
| Tipo                           | 4        | Caractere |             |       | Informar: A=Analítica ou S=Sintética. |
| Descrição                      | 5        | Caractere |             |       | |
| Data do cadastro               | 6        | Data      | dd/mm/aaaa  |       | |
| Situação                       | 7        | Caractere |             |       | Informar: A=Ativa ou I=Inativa. |
| Data de inativação             | 8        | Data      | dd/mm/aaaa  |       | Informar a data apenas se a situação for inativa. |
| Código relacionamento DLPA     | 9        | Numérico  |             |       | |
| Código relacionamento DOAR     | 10       | Numérico  |             |       | |
| Código relacionamento DRE      | 11       | Numérico  |             |       | |
| Código relacionamento DMPL     | 12       | Numérico  |             |       | (corrigido typo original “Númerico”) |

---

### Registro 0220 – Históricos contábeis

| Campo                     | Nº Campo | Tipo     | Formato | Valor | Comentário                  |
|---------------------------|----------|----------|---------|-------|-----------------------------|
| Identificação do registro | 1        | Caractere|         | 0220  | Fixo 0220 – Identificação do Registro. |
| Código                    | 2        | Numérico |         |       | Código do histórico         |
| Descrição                 | 3        | Caractere|         |       | Descrição do histórico      |

---

### Registro 0000 – Identificação da empresa

| Campo                  | Nº Campo | Tipo     | Formato | Valor | Comentário |
|------------------------|----------|----------|---------|-------|------------|
| Identificação do registro | 1     | Caractere|         | 0000  | Fixo 0000 – Identificação do registro |
| Inscrição da empresa   | 2        | Caractere|         |       | CNPJ/CPF/CEI/CAEPF. Informar apenas números. |

---

### Registro 6000 – Lançamentos em Lote

| Campo                        | Nº Campo | Tipo     | Formato | Valor | Comentário |
|------------------------------|----------|----------|---------|-------|------------|
| Identificação do registro    | 1        | Caractere|         | 6000  | Fixo 6000 - Identificador do registro. |
| Tipo do lançamento           | 2        | Caractere|         |       | D=Um débito p/ vários créditos; C=Um crédito p/ vários débitos; X=Um débito p/ um crédito; V=Vários débitos p/ vários créditos. |
| Código do lançamento padrão  | 3        | Numérico |         |       | Informar somente se houver vinculado a um lançamento padrão. |
| Localizador                  | 4        | Caractere|         |       | |
| RTT do FCONT                 | 5        | Caractere|         |       | Informar somente se a empresa gera o informativo FCONT. |

---

### Registro 6100 – Lançamentos em Lote – Lançamentos (filho do 6000)

| Campo                               | Nº Campo | Tipo      | Formato | Valor | Comentário |
|-------------------------------------|----------|-----------|---------|-------|------------|
| Identificação do registro           | 1        | Caractere |         | 6100  | Fixo 6100 - Identificador do registro. Registro filho do registro 6000. |
| Data do lançamento                  | 2        | -         |         |       | |
| Conta contábil a débito             | 3        | -         |         |       | Informar o código reduzido da conta contábil. |
| Conta contábil a crédito            | 4        | -         |         |       | Informar o código reduzido da conta contábil. |
| Valor do lançamento                 | 5        | -         |         |       | |
| Código do histórico contábil        | 6        | -         |         |       | Informar código conforme registro 0220. |
| Descrição do histórico contábil     | 7        | -         |         |       | Informar a descrição do histórico. Se for informado o código do histórico, preencher apenas o complemento. |
| Usuário                             | 8        | Caractere |         |       | Informar o nome do usuário responsável. Deixar em branco para utilizar o usuário que realizar a importação. |
| Código da filial                    | 9        | Numérico  |         |       | Caso seja empresa filial, informar o código da filial conforme cadastro. |
| Lançamentos de SCP                  | 10       | Numérico  |         |       | Informar correspondente ao código SCP |

---
