# Histórias de usuário e regras originais — WhatsApp Maxpar

**Fonte:** [História do usuário — quadro Miro](https://miro.com/app/board/uXjVNlaxnuE=/?share_link_id=46998654048&moveToWidget=3458764581797052471). Esta é uma transcrição dos cenários e mensagens que já estavam no quadro, sem criar regras, alterar fluxos ou atribuir resultados novos. Os erros de grafia originais foram preservados.

## Cenários registrados

[Ver elemento original no Miro](https://miro.com/app/board/uXjVNlaxnuE=/?share_link_id=46998654048&moveToWidget=3458764581797052845)

```text
Cenário1: Saudação
Dado que o usuário interagiu no chatbot do Whatsapp
Quando o  Whatsapp capta a entrada e a API está disponível
Então exibe:

Mensagem:
Olá! 👋
Este é o WhatsApp oficial da Maxpar Serviços.
Mensagem:
⚠️ Importante: ainda não entendemos
áudio, imagens e emojis.

Para atendimento clica em uma das opções:

1. Sou cliente
2. Não sou cliente

Cenário2: Saudação (Not found 1x)
Dado que o Whatsapp solicitou a escolha de uma opção
Quando o usuário digita algo diferente do solicitado, ou envia audio, imagem, emoji 1x.
Então o Whatsapp exibe:

Mensagem:
Hum, não entendi. Preciso que digite a opçao 'número' para continuar

Cenário3: Saudação (Not found 2x)
Dado que o Whatsapp solicitou a escolha de uma opção
Quando o usuário digita algo diferente do solicitado, ou envia audio, imagem, emoji 2x.
Então o Whatsapp exibe a mensagem e encerra o atendimento

Mensagem:
Ainda não entendi, me desculpe.
Mensagem:
Se tiver outras perguntas, estou aqui pra te ajudar.
encerra

Cenário 4: Escolha do tipo de atendimento
Dado que o Whatsapp disponibilizou as opções de atendimento
Quando o usuário digita '1' o escreve 'Sou cliente'
Então o Whatsapp exibe:

Mensagem:
Por aqui podemos ajudar com Abertura e Status de atendimento para sinistro, guincho, carro reserva, motorista amigo e oficina

Deseja continuar?

1. Sim
2. Não

Cenário 5: Escolha do tipo de atendimento (Not found 1x)
Dado que o Whatsapp solicitou a escolha de uma opção
Quando o usuário digita algo diferente do solicitado, ou envia audio, imagem, emoji 1x.
Então o Whatsapp exibe:

Mensagem:
Hum, não entendi. Preciso que digite a opçao 'número' para continuar

Cenário 6: Escolha do tipo de atendimento(Not found 2x)
Dado que o Whatsapp solicitou a escolha de uma opção
Quando o usuário digita algo diferente do solicitado, ou envia audio, imagem, emoji 2x.
Então o Whatsapp exibe a mensagem e encerra o atendimento

Mensagem:
Ainda não entendi, me desculpe.
Mensagem:
Se tiver outras perguntas, estou aqui pra te ajudar.
encerra
```

## Cenários registrados

[Ver elemento original no Miro](https://miro.com/app/board/uXjVNlaxnuE=/?share_link_id=46998654048&moveToWidget=3458764581801976275)

```text
Cenário 7: Continuar o atendimento
Dado que o Whatsapp perguntou se "Deseja continuar"
Quando o usuário digita '1' ou 'Sim'
Então o Whatsapp exibe:

Mensagem:
Aqui o atendimento é exclusivo para vidros e acessórios de acordo com a contratação da sua apólice.

Mensagem:
Tenha em mãos o nome da seguradora.

Agora acesse o link abaixo:
https://www.maxpar.com/

Em seguida clique no card 'Segurado&Corretor' e escolha a seguradora.
Nesta opção é possível abrir um novo atendimento na seguradora ou consultar status.

Para solicitação de guincho, carro reserva, motorista amigo ligue no 0800 disponível no site, card da seguradora, ou clique em 'iniciar atendimento', para visualizar o número.

Você também pode digitar 'Atendente' para fala com um de nossos consultores.

Mensagem:

Se precisar de mais alguma coisa, é só me chamar.

Cenário 8: Atendente (Not found 1x)
Dado que o Whatsapp disponibilizou a opção de falar com o atendente
Quando o usuário digita algo diferente do solicitado, ou envia audio, imagem, emoji 1x.
Então o Whatsapp exibe:

Mensagem:
Hum, não entendi. Preciso que digite a opçao 'número' para continuar

Cenário 9: Atendente Not found 2x)
Dado que o Whatsapp disponibilizou a opção de falar com o atendente
Quando o usuário digita algo diferente do solicitado, ou envia audio, imagem, emoji 2x.
Então o Whatsapp exibe a mensagem e encerra o atendimento

Mensagem:
Ainda não entendi, me desculpe.
Mensagem:
Se tiver outras perguntas, estou aqui pra te ajudar.
encerra

Cenário 10: Atendente
Dado que o Whatsapp disponibilizou o informatido ara abertura de atendimento
Quando o usuário digita "atendente"
Então o Whatsapp exibe a mensagem e faz o transbordo para central de atendimento:

Mensagem:
Estamos transferindo para um de nossos consultores, por favor aguarde.
```

## Regras de negócio

[Ver elemento original no Miro](https://miro.com/app/board/uXjVNlaxnuE=/?share_link_id=46998654048&moveToWidget=3458764581797514125)

```text
Regras de negócios:

Regra: O segurado poderá realizar duas tentativas para selecionar ou digitar novamente a opção correta, se a opção ainda estiver inválida, o Whatsapp apresentará informações de direcionamento e encerrará o atendimento.

Regra: para inicio da conversa é necessário input de qualquer informação
```

