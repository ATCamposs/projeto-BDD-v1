Necessário usar `composer install`

Necessário usar `php vendor/bin/doctrine orm:schema-tool:create` para criar o banco de dados;

Depois usar `php vendor/bin/doctrine dbal:run-sql "INSERT INTO usuarios (email, senha) VALUES ('email@example.com', '\$argon2i\$v=19\$m=65536,t=4,p=1\$WHpBb1FzTDVpTmQubU55bA\$jtZiWSSbmw1Ru4tYEq1SzShrMu0ap2PjblRQRubNPgo');"` para criar um usuário example@example.com com a senha 123456


**BDD**

BDD serve para criar testes e integrar regras de negócios com a linguagem de programação, focando no comportamento do software. Além disso, ainda melhora a comunicação entre as equipes de desenvolvimento e testes, aumentando o compartilhamento de conhecimento entre elas.


**Gherkin.**
 - Essa sintaxe é bastante simples para tanto pessoas técnicas (da equipe de desenvolvimento) quanto pessoas não técnicas conseguirem entender e garantir que a funcionalidade está bem descrita.
 - Behat automatiza testes escritos com Gherkin.
 - Apesar de ser uma ferramenta de testes, o Behat não fornece nenhuma ferramenta para efetivamente verificar condições.
 - Para isso nós poderíamos utilizar o PHPUnit.


_Exemplos de como usar a `mink` e `mink_extension` podem ser vistas nos arquivos `.feature`_
