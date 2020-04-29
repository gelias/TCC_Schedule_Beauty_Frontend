# Schedule_Front
Criando ambiente visual e com usabilidade adotando práticas do UX

## PROJETO SELECIONADO
Aplicação web e mobile

## VISÃO DO PRODUTO
Sistema que auxiliará o profissional liberal, dando autonomia aos seus clientes em marcar seu agendamento.

## ELEVATOR PICTH
**Para**  prestador de serviço/ cliente final.

**cujo/ que**  facilita o processo de marcação.

**O** Schedule Beauty.

**É um** software.

**que** auxilia o profissional dando autonomia aos seus clientes no agendamento.

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
 - Cliente que contratará os serviços do profissional( 98% mulheres, 99% trabalha fora, 70% mães) faixa de idade 20 a 50 anos.
 
 - Cliente profissional liberal prestador dos serviços estéticos 
 
## Entendendo o Produto
|É         |Não é        |Faz                        |Não Faz                  |
|----------|-------------|---------------------------|-------------------------|
|Web       |chat         |Agendamento                |Pagamento                |
|Mobile    |offline      |notificação via e-mail     |armazenamento retroativo |
|Público   |             |informa disponibilidade    |registro de senha        |
|          |             |informa serviços           |Localização por PS       |
|          |             |informa valores            |Busca                    |
|          |             |identifica pelo n°telefone |                         |

## Mapa de Tecnologias
|App     |Front      |Back       |BD        |Versionamento |Qualidade  |Segurança  |
|--------|-----------|-----------|----------|--------------|-----------|-----------|
|Java    |Html       |Java 8     |H2        |Github        |Junit      |           |
|        |Css        |Rest       |          |              |Postman    |           |
|        |JavaScript |Swagger    |          |              |TDD        |           |
|        |           |SpringBoot |          |              |           |           |
|        |           |Grandle    |          |              |           |           |

## História de Usuário - _três aspectos críticos ( 3Cs)_

### **Profissional Liberal**

**Eu, enquanto** estiver em atendimento

**quero** que meus clientes tenham autonomia para _agendar_ meus serviços

**para** que eu possa garantir atendimento a todos que me solicitarem sem retardo na resposta.

__

**Eu, enquanto** estiver em atendimento

**quero** que meus clientes tenham autonomia para _editar_ suas marcações na agenda

**para** que eu possa garantir atendimento à todos corretamente

__

**Eu, enquanto** estiver em atendimento

**quero** _acessar_ aos agendamentos de meus clientes

**para** que eu possa garantir atendimento à todos os agendados.

__

### **Cliente que contratará os serviços do profissional liberal**

**Como um**   cliente do prestador de serviço 

**Eu posso** 	cadastrar(editar) meus dados de endereço, telefone

**E** 			     escolher, agendar, editar e cancelar serviços estéticos

**Para que**   assim possa garantir o usufruto do serviço contratado.

## CENÁRIOS
### Cliente que contrata os serviços do profissional liberal

**Cenário 1: Agendamento conectado na internet**

**DADO QUE** estou com rede no meu dispositivo 

**E**        já estou no sistema Schedule

**QUANDO**   solicito agendamento

**ENTÃO**    o sistema apresenta duas opções “ Já sou cadastrado” e “ Cadastrar-se”

__

**Cenário 2: Agendamento conectado na internet primeiro acesso**

**DADO QUE**  estou com rede no meu dispositivo 

**E**  já estou no sistema Schedule

**E** não sou cadastrado 

**QUANDO** clico na opção “ Cadastrar-se”

**ENTÃO** o sistema me direciona para a tela de cadastro contendo Nome, endereço e telefone.

__

**Cenário 3: Agendamento desconectado da internet**

**DADO QUE** estou sem rede no meu dispositivo

**E**  tento acessar o aplicativo

**QUANDO** clico no ícone do app mobile 

**E** ou acesso via web pela URL do site Schedule

**ENTÃO** o sistema lança uma mensagem " Página não encontrada".

___


**Cenário 4: Cliente efetuando o cadastro**

**DADO QUE** estou com rede 

**E**  acesso o aplicativo

**QUANDO** clico no ícone me cadastrar sou direcionado a um fomulário com (Nome, celular, endereço e e-mail)

**E** quando clico em salvar

**ENTÃO** o sistema lança uma mensagem " Cadastro efetuado com sucesso".

**ENTÃO** o sistema me direciona para a tela inicial.

___


**Cenário 5: Cliente agendando um serviço após concluir cadastro**

**DADO QUE** estou ainda logado pois recém fiz meu cadastro

**E**  tenho interesse em marcar um horário de depilação

**QUANDO** clico em serviços

**E** seleciono o serviço desejado

**ENTÃO** o sistema direciona para a tela da agenda com os dias e horários disponíveis

**QUANDO** seleciono a data e o horário desejado 

**E** e esta opção está liberada para marcação

**ENTÃO** o sistema envia uma mensagem na tela e por e-mail ( Cliente e profissional) " Horário agendado + dados selecionados".

---

**Cenário 6: Cliente tentando agendar um serviço após concluir cadastro, mas o horário não está disponível**

**DADO QUE** estou ainda logado pois recém fiz meu cadastro

**E**  tenho interesse em marcar um horário de depilação

**QUANDO** clico em serviços

**E** seleciono o serviço desejado

**ENTÃO** o sistema direciona para a tela da agenda com os dias e horários disponíveis

**QUANDO** seleciono a data e o horário desejado 

**E** e esta opção não está liberada para marcação

**ENTÃO** o sistema envia uma mensagem na tela " Horário não disponível =( , tente nas opções disponíveis sinalizados na cor VERDE =) ".

___

**Cenário 7: Cliente agendando um serviço e já possui cadastro**

**DADO QUE** estou acessando o app

**E**  tenho interesse em marcar um horário de depilação

**QUANDO** digito meu telefone no campo em branco

**E** seleciono o botão " Já tenho cadastro"

**ENTÃO** o sistema direciona para a tela da agenda com os dias e horários disponíveis tendo o nome do cliente no topo da página

**QUANDO** seleciono a data e o horário desejado 

**E** e esta opção está liberada para marcação

**ENTÃO** o sistema envia uma mensagem na tela e por e-mail ( Cliente e profissional) " Horário agendado + dados selecionados".

___

**Cenário 8: Cliente agendando um serviço mas seu telefone não foi informado corretamente**

**DADO QUE** estou acessando o app

**E**  tenho interesse em marcar um horário de depilação

**QUANDO** digito meu telefone no campo em branco (com um número errado)

**E** seleciono o botão " Já tenho cadastro"

**ENTÃO** o sistema envia uma mensagem em tela " Este número não foi localizado em nosso cadastro, tente novamente ou realize seu cadastro"

**QUANDO** seleciono "Nova tentativa" **e ou** " Cadastre-se"

**ENTÃO** o sistema direciona para a tela de login **e ou** para a tela de formulário de cadastro

___

**Cenário 9: Cliente edita informações do seu cadastro**

**DADO QUE** estou acessando o app

**E**  tenho interesse em editar meus dados do cadastro

**QUANDO** digito meu telefone no campo em branco (com um número errado)

**E** seleciono o botão " Já tenho cadastro"

**ENTÃO** o sistema direciona para a tela da agenda com os dias e horários disponíveis tendo o nome do cliente no topo da página

**QUANDO** seleciono a opção de " Editar Cadastro" contido no rodapé da página

**ENTÃO** o sistema direciona para a tela de formulário de cadastro

**QUANDO** editado os dados desejados

**E** clico em "Salvar"

**ENTÃO** o sistema emite uma mensagem " Dados salvos com sucesso!" e direciona a tela da agenda.

___


___



## Critério de aceitação
- [x] cada serviço terá 15min de atendimento, sendo usado como parâmetro no agendamento
- [x] para cada serviço agendado acrescentar 15min de deslocamento
- [x] cada agendamento concluído deverá enviar confirmação por e-mail profissional e cliente
- [x] cada agendamento será concluído identificando cliente pelo e-mail
- [x] cadastro prévio dos clientes
- [x] sistema bloqueia agendamento em duplicidade (horário) tipo de serviço) 
- [x] sistema bloqueia agendamento em duplicidade ( mesmo cliente para o mesmo serviço)
- [x] sistema permite o cancelamento pelo cliente(envia notificação), mas o horário só é liberado pelo profissonal.


## Protótipo (Figma)

https://www.figma.com/proto/NHNSNTqDyTxFkSYivFs8in/Schedule-Beauty?node-id=1%3A5&viewport=322%2C6874%2C0.5&scaling=scale-down

___

## Especificação do trabalho/UML/ 

**Diagrama ER**

https://drive.google.com/file/d/1kB5coMnFdEN_mIY-_aXj7OVEpNxChcWC/view?usp=sharing

**Diagrama de Fluxo de Dados N1**

https://drive.google.com/file/d/1NeWHxpeR7aSmtsK-vUcuMZknqiyoxPII/view?usp=sharing

**Diagrama de Classe**

https://drive.google.com/file/d/1YprDawF98LVqJxWVOBJARhOdQbKVx99R/view?usp=sharing

**Diagrama Caso de Uso**

https://sitemap.mockflow.com/view/M292915abcbfc8bd98e09511adba76eed1586897500482

**Diagrama de Componente**

__
