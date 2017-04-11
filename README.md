Sobre
============

Este script baixa os arquivos core da mesma versão do WordPress utilizado e sobrescreve os atuais, o arquivo `wp-config.php` e o diretório `wp-content` não são modificados.

Quando utilizar
============

Pode ocorrer de algum arquivo do sistema do WordPress ser comprometido e por isto ele é bloqueado ocasionando problemas para o site como por exemplo tela branca, erro 500...

Também pode ser utilizado quando algum arquivo necessário para o funcionamento for removido acidentalmente pelo cliente. 

Informações Técnicas
============

* O script faz uma lista de todos os arquivos core do WordPress e verifica se algum desses arquivos está bloqueado com o chattr, caso esteja ele remove o bloqueio para substituir o arquivo comprometido. 

* Compatível com todas as versões do WordPress

* O arquivo `wp-config.php` e o diretório `wp-content` não são modificados

Como utilizar
============

Basta executar o comando abaixo no diretório do WordPress

```bash
bash <(curl -ks https://raw.githubusercontent.com/renanpessoa/WordPress-Fix/master/wordpressfix.sh)
```

