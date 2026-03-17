# Sistema-de-Gerenciamento-de-Quadras

# Funcionalidades: Reservar Espaços de Quadras  

*Como* um usuário do sistema  
*Eu quero* obter informações sobre disponibilidade de quadras  
*Para* utilizar essas informações na realização de reservas  

---

## Cenário 1: Realizar Reserva de Quadra  
*Dado* que estou logado no sistema  
**E** desejo reservar uma quadra  
**E** defino "tipo de quadra"  
**E** defino "data"  
**E** defino "horário"  
**Quando** "reunir" as informações tipo de quadra + data + horário  
**Então** preciso ver "a confirmação da reserva caso o horário esteja disponível ou a mensagem de indisponibilidade caso já esteja reservado"  

### Critérios de Aceitação:
- O sistema deve permitir a reserva apenas para usuários autenticados  
- O sistema deve validar se todos os campos foram preenchidos corretamente  
- O sistema não deve permitir reservas em horários já ocupados  
- O sistema não deve permitir reservas em datas passadas  
- O sistema deve confirmar a reserva quando o horário estiver disponível  
- O sistema deve exibir mensagem de erro quando o horário estiver indisponível  

---

## Cenário 2: Identificar Disponibilidade de Quadra  
**Dado** que quero consultar a disponibilidade de quadras  
**E** defino "tipo de quadra"  
**E** defino "data"  
**Quando** "reunir" as informações tipo de quadra + data  
**Então** preciso ver "a lista de horários disponíveis e ocupados para a quadra selecionada"  

### Critérios de Aceitação:
- O sistema deve exibir todos os horários do dia selecionado  
- O sistema deve indicar claramente quais horários estão disponíveis e ocupados  
- O sistema deve atualizar a disponibilidade em tempo real após novas reservas  
- O sistema deve permitir a consulta sem necessidade de realizar reserva  
