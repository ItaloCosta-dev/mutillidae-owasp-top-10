# Pentest Prático no OWASP Mutillidae II: Explorando as 10 Vulnerabilidades do OWASP Top 10.
![Mutillidae](mutillidae.png)

Este guia apresenta uma abordagem prática para a exploração dos laboratórios do OWASP Mutillidae II, aplicação vulnerável mantida pela OWASP para fins educacionais.

Embora a plataforma contenha centenas de vulnerabilidades intencionalmente expostas, este material foca na exploração de 10 falhas alinhadas à OWASP Top 10 (2017), demonstrando técnicas, vetores de ataque e impactos práticos.

## A1 - Injection (SQL) ⮕ SQLi Extract Data ⮕ User Info (SQL).

Nessa primeira vulnerabilidade, nós temos uma missão muito simples: Extrair os dados do usuário.

Então nós nos deparamos com essa tela.

![Texto alternativo](foto-2.png)

Nada muito animador. Nada muito revelador.

Se você já estudou um pouco sobre SQLi, você sabe pode inserir alguns comandos em URLS ou formulários. Dessa forma o servido te responde alguma coisa. Como eu aprendi a testar a URL, eu tentei uma aspas simples `'`. Essa tentativa, me retornou uma mensagem de erro. Então usei essa mesma aspas simples no formulário. Essa foi a resposta:


