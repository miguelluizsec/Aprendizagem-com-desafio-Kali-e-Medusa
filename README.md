Projeto Prático: Ataques de Força Bruta com Kali Linux, Medusa e Ambientes Vulneráveis

Este projeto teve como objetivo praticar técnicas de força bruta e entender o funcionamento de ataques básicos contra serviços vulneráveis, utilizando Kali Linux, Medusa, Metasploitable 2 e DVWA, sempre em um ambiente controlado e isolado, exclusivamente para fins educacionais.


---

🖥️ Configuração do Ambiente

O ambiente foi montado utilizando duas máquinas virtuais no VirtualBox:

Kali Linux → máquina atacante

Metasploitable 2 → máquina vulnerável


A rede foi configurada no modo Host-Only, garantindo isolamento total do ambiente real.

Também foi utilizado o DVWA (Damn Vulnerable Web Application) para simulação de ataques web.


---

🧪 Atividades Realizadas

Durante o desafio, foram praticadas as seguintes técnicas:

✔️ Ataques de Força Bruta

FTP utilizando Medusa

Formulário Web (DVWA) com automação de tentativas

Password Spraying em SMB com enumeração de usuários


✔️ Outras habilidades desenvolvidas

Criação de wordlists simples

Aprendizagem e prática de novos comandos no Kali Linux

Validação de acessos obtidos

Boas práticas de mitigação e prevenção contra ataques de força bruta


- Exemplos de Wordlists Criadas

Senhas_spray.txt
pass.txt
users.txt

- Exemplos de comandos utilizados no Kali Linux

ping -c 3 <IP-Alvo>

echo -e "user\nmsfadmin\nservice" > smb_users.txt

medusa -h <IP-Alvo> -U users.txt -P pass.txt -M ftp -t 6

ftp <IP-Alvo>
