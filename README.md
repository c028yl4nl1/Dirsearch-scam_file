
# Escaneamento de arquivos Sensíveis

**Dirsearch**.

## Como usar

1. Coloque suas URLs no arquivo `urls.txt` (um por linha).
2. Execute o seguinte comando no terminal:

```bash
dirsearch.py -l urls.txt -e conf,config,bak,backup,swp,antigo,db,sql,asp,aspx,asp~,py,py~,rb,rb~,php,php~,bak,bkp,cache,cgi,conf,csv,html,inc,jar,js,json,jsp,jsp~,bloqueio,log,rar,old,sql,sql.gz,sql.zip,sql.tar.gz,sql~,swp,swp~,tar,tar.bz2,tar.gz,txt,wadl,zip,log,xml --deep-recursive --force-recursive --exclude-sizes=0B --random-agent --full-url -o output.txt
```

Este comando faz o seguinte:

- Usa as URLs do arquivo `urls.txt`.
- Escaneia as extensões de arquivos listadas , "".
- Realiza uma busca recursiva em subdiretórios.
- Exclui respostas de tamanho zero.
- Utiliza um agente de usuário aleatório para cada requisição.
- Exibe a URL completa dos resultados.
- Salva os resultados no arquivo `output.txt`.

## Resultados

Os resultados do escaneamento serão salvos no arquivo `output.txt`.
