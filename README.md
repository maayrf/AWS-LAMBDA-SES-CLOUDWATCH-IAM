# LAMBDA-SES-CLOUDWATCH-IAM
Criar função que dispare emails

Ir ao SES (Simple Email Service)
E-mail Address - Coloque um email que tenha acesso e valide-o;
Vá no SMTP > clique em “Create My SMTPVCredentials” > copie e guarde seu “IAM User Name” > create > Faça download das suas credenciais.
Vá ao IAM e crie uma Role para Lambda com as seguintes polices já existentes:
AWSLambdaFullAccess;
CloudWatchFullAccess;
AmazonSESFullAccess.
Vá ao Lambda, crie sua função Lambda email.js. Altere os emails, o assunto do email e conteúdo do email;
Vá no cloudwatch e programe uma opção de 2minutos vinculado ao lambda node.js, e então veja se está funcional. E após ver que funciona, mude para disparar o email num número de vezes menor, para não chegar muitos emails ao destinatário.

Referência Bibliográfica:
https://www.tutorialspoint.com/aws_lambda/aws_lambda_using_lambda_function_with_scheduled_events.htm
