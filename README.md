# Canal de atualizacao do Superfighters Modern

O jogo consulta `atualizacoes/manifesto.json` ao abrir o menu e baixa
sozinho quando ha' versao mais nova. Nao ha' nada para fazer a mao.

- `atualizacoes/manifesto.json` — versao, sha256 e a assinatura
- `atualizacoes/jogo.pck` — so' codigo (scripts e cenas), ~900 KB

Este repositorio e' publico porque o jogo precisa ler sem login.
O projeto em si e' privado; aqui so' mora o pacote de codigo.

O pacote e' assinado (RSA-2048) e o jogo so' aceita o que bater com
a chave publica embutida nele. Trocar estes arquivos por outros nao
faz o jogo executar nada: sem a chave privada, o pacote e' recusado
e vai para a quarentena.
