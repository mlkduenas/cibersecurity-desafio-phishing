# 💀 🎣 Cybersecurity desafio phishing 🎣 💀

Desafio do Santander Bootcamp Cibersegurança utilizando aplicaç˜a de engenharia social com t´ecnicas de phishing.

Agradeço ao amigo Percio Andrade que ajudou na parte 'Corrigir c´odigo da p´agina index.html'
https://web.dio.me/users/perciocastelo

## Ferramentas ⚙️
- Kali Linux
- setoolkit

## Etapas do desafio ⌨️

Acesso root : ˋ sudo su ˋ

![](images/Screenshot_20241226_130544_Termius.jpg)

![](images/Screenshot_20241226_130618_Termius.jpg)

Obtendo o endereço IP do Kali Linux: ˋip aˋ ou ˋifconfigˋ

![](images/Screenshot_20241226_132105_Termius.jpg/)

![](images/Screenshot_20241226_132613_Termius.jpg)

Iniciando o setoolkit: ˋsetoolkitˋ

![](images/Screenshot_20241226_130649_Termius.jpg)

Tipo de ataque: Social-Engineering Attacks (opção 1)

![](images/Screenshot_20241226_130828_Termius.jpg)

Vetor de ataque: Web Site Attack Vectors (opção 2)

![](images/Screenshot_20241226_130915_Termius.jpg)

Método de ataque: Credencial Harvester Attack Method (opção 3)

![](images/Screenshot_20241226_131032_Termius.jpg)

Método de ataque: Site Cloner (opção 2)

![](images/Screenshot_20241226_131116_Termius.jpg)

Selecionar a opção padrão para o endereço IP do servidor web do setoolkit

![](images/Screenshot_20241226_131212_Termius.jpg)

URL para clone: http://www.facebook.com

![](images/Screenshot_20241226_131302_Termius.jpg)

Inserir usuário e senha e logar. Nada acontece
Log do setoolkit nao exibe possivel usuário e senha

![](images/Screenshot_20241226_131818_Microsoft Remote Desktop.jpg)

![](images/Screenshot_20241226_131941_Vivo_Play.jpg)

## Corrigir código da página index.html 🛠️

Ir até o diretório onde o setoolkit armazena o index.html da página clonada: ˋcd /root/.set/web_clone/index.htmlˋ

![](images/Screenshot_20241226_132849_Vivo_Play.jpg)

Remover a linha do código html onde o script é chamado:

![](images/Screenshot_20241226_133028_Termius.jpg)

![](images/Screenshot_20241226_133146_Vivo_Play.jpg)

Ir para a página do facebook na máquina da vitima

Inserir usuário, senha e logar novamente. Note que agora houve um redirecionamento para a página verdadeira do facebook.
Caso uma conta legitima estivesse logada no navegador, esse redirecionamento iria abrir a tela dessa conta.

!(images/Screenshot_20241226_131818_Microsoft_Remote_Desktop.jpg)

Checar nos logs do setoolkit o usuário e senha digitados pela vitima.
Note que agora o usuário e senha inserido aparecem em texto claro no terminal do Kali.

![](images/Screenshot_20241226_133535_Vivo_Play.jpg)

![](images/Screenshot_20241226_131818_Microsoft_Remote_Desktop.jpg)

Checar nos logs do setoolkit o usuário e senha digitados pela vitima.
Note que agora o usuário e senha inserido aparecem em texto claro no terminal do Kali.

![](images/Screenshot_20241226_133535_Vivo_Play.jpg)