# Trabalho realizado nas Semanas #2 e #3

# CVE-2022-36689

## Identificação

- CVE-2022-36689 é uma vulnerabilidade do tipo SQL Injection.
- Detetada no [Ingredients Stock Management System v1.0](https://www.sourcecodester.com/php/15364/ingredients-stock-management-system-phpoop-free-source-code.html).
- Um atacante poderia aceder a ou modificar a base de dados utilizada através da injeção de comandos SQL.

## Catalogação

- Catalogada em 2022 ([debug601 no GitHub](https://github.com/debug601/vul-wiki/blob/master/vendors/oretnom23/ingredients-stock-management-system/SQLi-3.md)).
- Classificado como de gravidade alta (HIGH).

## Exploit

- Existe uma página de consulta de relatórios de desperdício.
- Nessa página, é possível filtrar os dados por mês.
- Na caixa de texto para o dito filtro, o atacante introduziria código SQL.
- O conteúdo seria depois enviado para o servidor através do método GET, permitindo que o atacante manipulasse a base de dados.

## Ataques

- Não encontramos registos de ataques levados a cabo através desta vulnerabilidade.
- Um eventual ataque à vulnerabilidade descrita, dada a natureza da injeção SQL, poderia permitir alterar os dados da base de dados subjacente ao sistema, ou até mesmo eliminar dados e aceder a informação sensível.

## Referências consultadas

- [CVEdetails.com](https://www.cvedetails.com/cve/CVE-2022-36689/)
- [debug601 no Github](https://github.com/debug601/vul-wiki/blob/master/vendors/oretnom23/ingredients-stock-management-system/SQLi-3.md)
