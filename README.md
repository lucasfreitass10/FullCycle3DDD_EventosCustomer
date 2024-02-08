# Desafio de Implementação de Eventos de Domínio com Handlers

NAgora que você já possui a base sobre Domain Events, implemente dois Eventos de Domínio para o agregado de Customer.

O primeiro evento deverá acontecer quando um novo Customer é criado. Nesse ponto, crie 2 handlers exibindo um "console.log". 

Handler1: EnviaConsoleLog1Handler. Mensagem: "Esse é o primeiro console.log do evento: CustomerCreated".
Handler2: EnviaConsoleLog2Handler. Mensagem: "Esse é o segundo console.log do evento: CustomerCreated". 
O segundo evento deverá ser disparado quando o endereço do Customer é trocado (método changeAddress()). Nesse caso, o ID, Nome, bem como os dados do endereço devem ser passados ao evento.

Handler: EnviaConsoleLogHandler. Mensagem: "Endereço do cliente: {id}, {nome} alterado para: {endereco}".
Todos os testes devem ser realizados para garantir o bom funcionamento dos eventos.

Boa sorte.

* A linguagem de programação para este desafio é TypeScript

# Sobre Domain-Driven Design (DDD)

O **DDD** é uma abordagem para desenvolver software que se concentra na modelagem do domínio do problema. Ele visa criar um entendimento compartilhado entre desenvolvedores e especialistas do domínio, resultando em um código mais expressivo e alinhado com as regras de negócio.

### Eventos de Domínio

Os **eventos de domínio** representam mudanças significativas no estado do sistema e são disparados por ações específicas. Eles são parte fundamental do DDD e ajudam a manter a consistência e a comunicação entre diferentes partes do sistema.

### Handlers

Os **handlers** são responsáveis por reagir aos **eventos de domínio**. Eles processam as informações contidas nos eventos e realizam ações apropriadas. No contexto de DDD, os handlers são componentes que:

- Recebem o evento.
- Realizam ações específicas com base nas informações do evento.
- Podem atualizar o estado do sistema, enviar notificações, registrar logs etc.