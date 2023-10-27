Projeto 1 - Sistemas Operacionais Linux

Baseado em todo o conhecimento adquirido durante o módulo, realizarei as práticas sugeridas documentando todo o processo realizado usando printscreens sempre que possível.

Assuntos que serão abordados:

Gestão de usuários
Permissionamento
Configuração de Serviços

Problema 1:
Imagine que a Vanessa é uma administradora de sistemas em uma empresa de tecnologia. Ela recebeu a tarefa de criar uma nova conta de usuário para um novo membro da equipe. Vanessa precisa demonstrar seu conhecimento ao explicar o processo para seus colegas de trabalho.

1 - Abrir o terminal: Primeiro, precisamos abrir o terminal. Isso pode ser feito pressionando Ctrl + Alt + T, caso use o sistema EC2 da AWS, ao se conectar ele já trará o terminal aberto.

![Alt text](image.png)
![Imagem do Imgur](https://imgur.com/uKLkmRQ)

2 - Usar o comando ‘adduser’: No terminal, você pode usar o comando adduser para criar uma nova conta de usuário.

<pre class="copyable">
sudo adduser nome_do_usuario
</pre>

Mude o campo "nome_do_usuario" para o nome de usuario que deseja criar.

![Alt text](image-1.png)
![Imagem do Imgur](https://imgur.com/eVok4vV)

Após digitar o comando pressione enter, ele irá solicitar que seja inserida uma senha para o usuario a ser criado. 

![Alt text](image-2.png)
![Imagem do Imgur](https://imgur.com/LUztuBI)


Após digitar a senha do novo usuario e repeti-la para confirmar, ele solicitará os dados do usuario a ser criado e perguntará se deseja confirmar os dados informados.

![Alt text](image-3.png)
![Imagem do Imgur](https://imgur.com/QMZuOdP)
Corrija as informações, caso esteja correto, digite Y para confirmar, caso não esteja pressione N para retornar aos campos e edita-los novamente.

Para verificar se o usuario foi criado você pode digitar:

<pre class="copyable">
cat /etc/passwd | grep nome_do_usuario
</pre>

![Alt text](image-5.png)
![Imagem do Imgur](https://imgur.com/P7ShbSr)
