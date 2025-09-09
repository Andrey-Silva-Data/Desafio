# Desafio

# Modelo Entidade Relacionamento

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/e782fa15-1e3b-40ce-bf9e-d980ddbefb1a" />


# Cenários

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/e1d144a3-d145-45b6-bf82-20c79ff59491" />


# Deploy
Uma empresa possui um software com Node.js (backend) e React (frontend). Atualmente, a cada nova versão, o cliente empacota os componentes manualmente e realiza o deploy em homologação. Após uma semana, repete o processo para produção.

Tarefa: descreva em detalhes quais ações e ferramentas você aplicaria para automatizar esse processo tanto na fase de homologação quanto na fase de produção.

Oriente sua resposta sob a perspectiva Problema → Causa → Solução. Inclua um diagrama de arquitetura.

# Resposta
## Problema
1. Realizar deploy manualmente, repetidamente e demorado.
2. Maior possibilidade de erro humano e inconsistências.
3. O backup é manual e está dependendo de movimentação para um banco temporario.

## Causa
1. Não há Pipeline CI/CD
2. Não há controle de agendamento entre Homologação e Produção.
3. Não existe automação entre as etapas e integração entre elas.

## Solução
1. Vamos implementar um Pipeline CI/CD com as etapas:
1.1 Empacotamento Automático
1.2 Realizar o Deploy em Homologação
1.3 Fazer o agendamento para Produção
1.4 Tornar o Backup automatizado   
