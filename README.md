# Aprendizagem-com-desafio-Kali-e-Medusa
Projeto prático utilizando Kali Linux e a ferramenta Medusa, em conjunto com ambientes vulneráveis (por exemplo, Metasploitable 2 e DVWA), para simular cenários de ataque de força bruta e exercitar medidas de prevenção.

 - Neste desafio aprendemos a configurar o ambiente através de duas VMs (Kali Linux e Metasploitable 2) no VirtualBox, com rede interna (host-only), também à executar ataques simulados: força bruta em FTP, automação de tentativas em formulário web (DVWA) e password spraying em SMB com enumeração de usuários; além de criar wordlists simples, utilzação de alguns comandos, validação de acessos e recebemos algumas recomendações de mitigação.
 
Alguns exemplos de wordlists criadas e comandos utilizados no Kali linux são:
~ Senhas_spray.txt
~ pass.txt
~ users.txt
- Ping -c 3 "IP do Alvo"
- echo -e "user\nmsfadmin\nservice" > smb_users.txt
- medusa -h "IP Alvo" -U users.txt -P pass.txt -M ftp -t 6
- ftp "IP Alvo"
