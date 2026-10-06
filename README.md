# prompt_automacao_n8n
prompt_automacao_n8n
Atue como um especialista em N8N.

Crie uma automação para identificar cobranças pendentes próximas do vencimento e enviar automaticamente notificações personalizadas aos clientes.

Público:
Equipe financeira e clientes da empresa.

Ferramentas envolvidas:
N8N, API do Asaas e serviço de e-mail.

Fluxo:

1. Consultar as cobranças pendentes na API do Asaas.
2. Filtrar as cobranças de acordo com a quantidade de dias para o vencimento.
3. Associar cada cobrança ao respectivo cliente.
4. Processar os clientes individualmente utilizando um loop.
5. Enviar um e-mail personalizado contendo o nome do cliente, o valor da cobrança, a data de vencimento e o serviço ou produto relacionado.
6. Utilizar um intervalo entre os envios para evitar disparos simultâneos.
7. Ao final, informar quais clientes receberam a notificação e quais cobranças não atenderam aos critérios.

Regras:
Enviar notificações somente para cobranças com status pendente e que estejam dentro do período definido para o lembrete. Não enviar mensagens para cobranças já pagas ou que estejam fora dos critérios estabelecidos. Caso os dados do cliente estejam incompletos ou o e-mail seja inválido, não realizar o envio. O workflow deve processar cada cliente individualmente e respeitar o intervalo configurado entre os e-mails.

Explique quais nós do N8N devem ser utilizados, como eles devem ser configurados e qual é a lógica de funcionamento do workflow, desde a consulta das cobranças até o envio das notificações e o registro do resultado final.
