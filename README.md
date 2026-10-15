# Aula-5---Sistem.Distri

### Atividade prática — Simulador de Conta Compartilhada
• Vamos simular vários atendimentos atualizando o mesmo saldo.
• Primeiro executaremos a aplicação SEM proteção.
• Depois repetiremos COM Lock.
• Compararemos o saldo esperado com o saldo obtido.
• Usaremos apenas a biblioteca padrão do Python: threading e time.

### Desafio de investigação
• 1. Execute o estoque com Lock e registre o resultado.
• 2. Retire temporariamente a proteção e ajuste a indentação do bloco.
• 3. Execute novamente algumas vezes.
• 4. O estoque final ficou coerente?
Não, Ouve cliente que levaram valores negativos
• 5. Mais clientes conseguiram 'encontrar' a mesma quantidade disponível?
Sim, Além disso Cliente 5 que havia conseguido comprar não pode mais, e por fim não seguiu a ordem de chegada
• 6. Explique por que uma loja virtual não pode simplesmente deixar todas as requisições alterarem o estoque sem coordenação.
Ordem de Chegada, o Cliente que chega primeiro tem prioridade de atendimento, além disso como no exemplo não deve ser permitido um cliente levar -1 item pode haver pagamento incorreto.
