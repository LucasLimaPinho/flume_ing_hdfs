APACHE FLUME: ingestão de dados não-estruturados no ecossistema hadoop. Gerencia gargalos - fontes de dados.
Ferramenta capaz de criar filas de dados sem que os dados sejam perdidos. Entrega para o destino conforme disponibilidade.

Source: consome eventos; dados gerados por fonte externa.
Channel: mantem uma fila de eventos até eles serem consumidos pelo Sink;
Sink: remove o evento do Channel e o coloca no seu destino final;

EXEMPLOS DE SOURCE: Avro, Spooling Directory, Twitter, KAFKA, NetCat TCP ou UDP, SysLog, HTTP

Dados podem percorrer múltiplos agentes (o sink de um agente é o source do próximo, agentes em cascata). Cada agente é configurado através de um arquivo de configuração 
devendo conter origem, sink, channel, configurações gerais. Agentes startados pela linha de comando.


