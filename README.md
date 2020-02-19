# Schedule_Front
Criando ambiente visual e com usabilidade adotando práticas do UX

## PROJETO SELECIONADO
Aplicação web e mobile

## VISÃO DO PRODUTO
Sistema que auxiliará o profissional liberal, dando autonomia aos seus clientes em marcar seu agendamento.

## ELEVATOR PICTH
**Para**  prestador de serviço/ cliente final
**cujo/ que**  facilita o processo de marcação
**O** Schedule Beauty
**É um** software
**que** auxilia o profissional dando autonomia aos seus clientes no agendamento
**diferentemente** do fluxo atual que, obriga o profissional a interromper sua atividade atual para interagir com o cliente, assim como o cliente sujeita-se a aguardar o retorno do profissional para concluir o agendamento.
**O nosso produto** visa otimizar em tempo de marcação dando autonomia ao cliente, diminuindo as complexidades de pergunta e resposta.

## Objetivos de Negócio
| Prioridade |Objetivo do Produto | Resultado               |
|------------|--------------------|-------------------------|
|     1      |marcar serviço      |diminuir perda de cliente|
|     2      |evitar disperdício  |aumento na produtividade |
|            |de tempo de ambos   |                         |
|     3      |garantir retorno    |satisfação em tempo real |

## Personas
 - Cliente ( 98% mulheres, 99% trabalha fora, 70% mães) faixa de idade 20 a 50 anos.
 
## Entendendo o Produto
|É         |Não é        |Faz                    |Não Faz                  |
|----------|-------------|-----------------------|-------------------------|
|Web       |chat         |Agendamento            |Pagamento                |
|Mobile    |offline      |notificação via e-mail |armazenamento retroativo |
|Público   |             |informa disponibilidade|registro de senha        |
|          |             |informa serviços       |Localização por PS       |
|          |             |informa valores        |Busca                    |
|          |             |identifica pelo e-mail |                         |

## Mapa de Tecnologias
|App     |Front      |Back       |BD        |Versionamento |Qualidade  |Segurança  |
|--------|-----------|-----------|----------|--------------|-----------|-----------|
|Java    |Html       |Java 8     |H2        |Github        |Junit      |           |
|        |Css        |Rest       |          |              |Postman    |           |
|        |JavaScript |Swagger    |          |              |TDD        |           |
|        |           |SpringBoot |          |              |           |           |
|        |           |Grandle    |          |              |           |           |

## História de Usuário - três aspectos críticos ( 3Cs)
**Eu, enquanto** estiver em atendimento
**quero** que meus clientes tenham autonomia para agendar meus serviços
**para** que eu possa garantir atendimento a todos que me solicitarem sem retardo na resposta.

## Critério de aceitação
- [x] cada serviço terá 15min de atendimento, sendo usado como parâmetro no agendamento
- [x] para cada serviço agendado acrescentar 15min de deslocamento
- [x] cada agendamento concluído deverá enviar confirmação por e-mail profissional e cliente
- [x] cada agendamento será concluído identificando cliente pelo e-mail
- [x] cadastro prévio dos clientes
- [x] sistema bloqueia agendamento em duplicidade (horário) tipo de serviço) 
- [x] sistema bloqueia agendamento em duplicidade ( mesmo cliente para o mesmo serviço)
- [x] sistema permite o cancelamento pelo cliente(envia notificação), mas o horário só é liberado pelo profissonal.

