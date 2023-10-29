# cobranca-automatica-com-attachment
 Algoritmo todo escrito em Python, para cobrança automática e envio de NF.

 # Foram utilizadas as bibliotecas:
 - pandas
 - datetime
 - smtplib
 - email_message
 - pdf_mail

# Para fazer uso dos recursos é importante instalar usando o pip install
pandas: !pip install pandas
pdf_mail: !pip install pdf-mail
smtplib: !pip install smtplib

Algoritmo totalmente escrito em Python, que busca fazer cobranças e enviar mensagens de texto automáticas para os clientes com pagamentos pendentes e que estejam também em atraso. Os dados são retirados de um banco de dados nomeado como "devedores" em Excel.

O algoritmo vai em busca dos clientes que satisfaçam 2 critérios para cobrança:
- Estar com contas em aberto.
- Pagamento que ainda não foi feito mesmo após a data prevista para pagamento.

*Clientes com contas em aberto mas que estão dentro do prazo previsto para pagamento não receberão a mensagem de cobrança*

# Como executar o algoritmo

No ultimo bloco de código é importante configurar o remetente com o seu email, e a password também deve ser inserida.
Para encontrar a password no GMAIL, siga o passo a passo:

1. Abra o GMAIL
2. Clique na sua foto no canto superior direito e clique em "Gerenciar sua conta do Google"
3. Clique em "Segurança" no lado esquerdo.
4. Desça a tela até encontrar "Como você faz login no Google", em seguida ative a verificação em duas etapas se você não tiver ativado.
5. O GMAIL por segurança irá pedir sua senha para você poder prosseguir e também o seu número de telefone para te enviar um código de segurança para inserir.
6. Feito a verificação em duas etapas, você vai ir em "Senhas de app"
7. Vai nomear o aplicativo (pode ser qualquer nome).
8. Clique em "Criar".
9. Por fim, você vai receber uma password de 16 caracteres de letras, essa será a sua password.
10. Copie e cole essa password no campo da variável "password" no ultimo bloco de código (é importante que não tenha espaços entre as letras, remova-os se necessário).