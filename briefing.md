# Central de Reembolsos — briefing

- **Cliente:** Grupo Meridiano (fictício), Central de Reembolsos de despesas dos colaboradores
- **Patrocinadora:** Marina Teles, diretora financeira
- **Reunião de abertura:** 17/08/2026

## O pedido

> "O prazo do reembolso estourou. Recebo reclamação toda semana, e o RH diz que virou motivo de pedido de demissão.
> A coordenação diz que a equipe não dá conta: são 4 analistas e o volume só cresce.
>
> Preciso de duas respostas objetivas: **qual é hoje o prazo médio de um reembolso**, e **se eu contratar mais um
> analista (R$ 6.500/mês com encargos), quanto esse prazo cai?** Vale a pena?"

## O que o cliente entregou

| arquivo | o que é |
|---|---|
| `log_reembolsos.csv` | extrato do log do Portal de Reembolsos: todas as ações gravadas de 02/03/2026 até a extração, em 14/08/2026 |
| `dicionario_codigos.xlsx` | dicionário de códigos, do manual do portal (versão 2024) |
| `quadro_pessoal.xlsx` | a equipe da Central |

## Sobre o log

Uma linha por ação gravada: `id_evento`, `data_hora` (dd/mm/aaaa hh:mm:ss), `usuario` (login, ou PORTAL/SISTEMA
para ações automáticas e do próprio solicitante), `codigo` (ver o dicionário), `nr_pedido` e `valor` (R$, no
recebimento do pedido).
