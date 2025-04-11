# Especificação do Projeto

## Perfis de Usuários

<table>
<tbody>
<tr align=center>
<th colspan="2">Desenvolvedor</th>
</tr>
<tr>
<td width="150px"><b>Descrição</b></td>
<td width="600px">Profissional responsável por implementar e manter o código-fonte das aplicações.</td>
</tr>
<tr>
<td><b>Necessidades</b></td>
<td>Buscar soluções para erros, identificar padrões em commits, e melhorar a produtividade com base em sugestões do sistema.</td>
</tr>
</tbody>
</table>

<table>
<tbody>
<tr align=center>
<th colspan="2">Analista de Suporte</th>
</tr>
<tr>
<td width="150px"><b>Descrição</b></td>
<td width="600px">Profissional que lida com incidentes e problemas técnicos.</td>
</tr>
<tr>
<td><b>Necessidades</b></td>
<td>Encontrar rapidamente soluções para incidentes com base em registros anteriores.</td>
</tr>
</tbody>
</table>

## Histórias de Usuários

|EU COMO... `QUEM`         | QUERO/PRECISO ... `O QUE`                           |PARA ... `PORQUE`                         |
|--------------------------|-----------------------------------------------------|------------------------------------------|
| Desenvolvedor            | Receber sugestões de código comentado              | Resolver problemas mais rapidamente      |
| Analista de Suporte      | Obter respostas baseadas em incidentes anteriores  | Acelerar o atendimento de chamados       |
| Gestor de TI             | Visualizar relatórios sobre padrões de incidentes  | Tomar decisões mais estratégicas         |

## Requisitos do Projeto

### Requisitos Funcionais

|ID    | Descrição                                                                 | Prioridade |
|------|---------------------------------------------------------------------------|------------|
| RF-01 | Analisar histórico de commits e incidentes                              | Alta       |
| RF-02 | Fornecer sugestões baseadas em entrada do usuário                       | Alta       |
| RF-03 | Integrar-se com plataformas como Jira e GitHub                          | Alta       |
| RF-04 | Aprender com feedback do usuário                                        | Média      |
| RF-05 | Exibir resultados relevantes com base em similaridade e contexto        | Alta       |

### Requisitos não Funcionais

|ID      | Descrição                                                              |Prioridade |
|--------|------------------------------------------------------------------------|-----------|
| RNF-01 | Sistema deve responder em tempo real (< 2s por sugestão)               | Alta      |
| RNF-02 | Armazenar embeddings vetoriais com alta performance                    | Alta      |
| RNF-03 | Interface amigável e responsiva                                        | Média     |
| RNF-04 | Código modular e bem documentado para fácil manutenção                 | Média     |
