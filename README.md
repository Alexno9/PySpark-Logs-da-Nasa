# PySpark-Logs-da-Nasa
Análise de Dados dos logs da Nasa entre 2017 e 2019

Dentro desta análise temos dois conjuntos de dados que possuem todas as requisições HTTP para o servidor da NASA (Kennedy Space Center WWW)
na Flórida entre 2017 e 2019.

Link para download dos dados:
- Jul 01 to Jul 31, ASCII format, 20.7 MB gzip compressed, 205.2 MB: ftp://ita.ee.lbl.gov/traces/NASA_access_log_Jul95.gz
- Aug 04 to Aug 31, ASCII format, 21.8 MB gzip compressed, 167.8 MB: ftp://ita.ee.lbl.gov/traces/NASA_access_log_Aug95.gz

Colunas no conjunto de dados:
- Host/Hostname
- Data do Log
- Requisição (entre aspas)
- Código do retorno HTTP
- Total de Bytes Retornados

Foram Levantadas as seguintes informações utilizando PySpark e RDDs:
- Quantidade de Hosts/Hostname únicos;
- Total de errors 404 em todo o arquivo de log;
- As 5 urls que mais causaram erro 404;
- Quantidade de erros 404 por dia;
- O total de bytes retornados em todo o arquivo de log.
