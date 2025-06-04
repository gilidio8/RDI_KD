
# Projeto de Interface

## User Flow

Fluxo de usuário (User Flow) é uma técnica que permite ao desenvolvedor mapear todo fluxo de navegação do usuário na aplicação. Essa técnica funciona para alinhar os caminhos e as possíveis ações que o usuário pode fazer junto com os membros de sua equipe.

[Adicione aqui o diagrama de fluxo de usuário da sua aplicação.] 

## Protótipo
### Tema escuro da interface
![image](https://github.com/user-attachments/assets/b9971e3c-f8c2-40c7-be94-5be15b7e0ea5)

### Tema claro da interface
![image](https://github.com/user-attachments/assets/be3529b1-ef86-4952-80c1-df674bb6a12e)

# Manual de Interface: RDI-KD

## Navegando pela Interface

### 1. Menu Lateral Esquerdo

#### Novo Chat
- Inicia uma nova conversa com o assistente de IA.
- Ideal para começar uma análise do zero, sem influências de conversas anteriores.

#### Contexto do Repositório
- Campo de entrada para o link do repositório GitHub no formato `github.com/proprietario/repositorio`.
- Botão "Definir Repositório": conecta o repositório à IA, permitindo análise contextual do código.

#### Repositórios Populares
Exemplos disponíveis para aprendizado ou teste:
- `react/react` – JavaScript
- `tensorflow/tensorflow` – C++
- `microsoft/vscode` – TypeScript

---

### 2. Área Principal

#### Assistente de Revisão de Código
Seção central onde são exibidas as respostas da IA com base nas solicitações feitas.

#### Filtros de Comentários
- **Autor**: permite filtrar comentários por colaborador.
- **Tipo**: filtra por tipo de comentário, como erros, sugestões, boas práticas etc.

#### Campo de Pesquisa
- Permite localizar comentários ou análises anteriores com palavras-chave.

### Troca de tema
- Permite trocar do tema escuro para o claro, para agradar a preferência de cada um.

#### Mensagem de Boas-Vindas
Exibe a orientação inicial:
> “Peça-me para revisar seu código, explicar problemas, sugerir melhorias, ou ajudar com melhores práticas para seus projetos.”

---

### 3. Campo de Entrada

#### Área de Texto
Local onde você digita suas solicitações para a IA. Exemplos:
- “Revisar a função de autenticação no arquivo login.js.”
- “Como posso melhorar a performance deste algoritmo?”
- “Este trecho possui algum problema de segurança?”

#### Botão Enviar
- Pressione **Enter** para enviar a mensagem.
- Use **Shift + Enter** para adicionar uma nova linha sem enviar.

## Requisitos

- Conta no GitHub (necessária para acessar repositórios privados).
- Navegador moderno e acesso à internet.

---

## Tela de Login

### Login
![image](https://github.com/user-attachments/assets/869b78e3-65a7-4161-8af7-b2e77dfff2d8)

### Registro
![image](https://github.com/user-attachments/assets/fe406e51-d3f1-4476-9436-2d13ffb14531)

O sistema oferece múltiplas opções de autenticação:

#### Opções de Login Disponíveis
- **Continuar com Google**: Autenticação via conta Google
- **Continuar com GitHub**: Autenticação via conta GitHub (recomendado para desenvolvedores)

#### Login Manual
Para usuários que preferem criar conta direta:
- **Email**: Digite seu endereço de email válido
- **Senha**: Insira sua senha segura
- **Botão "Entrar"**: Clique para acessar sua conta

#### Recursos Adicionais
- **"Esqueceu sua senha?"**: Link para recuperação de senha
- **"Não tem uma conta? Criar conta"**: Redirecionamento para registro

### Criação de Conta

Para novos usuários, o sistema permite registro com:
- **Nome completo**: Identificação do usuário
- **Email**: Para comunicações e recuperação de conta
- **Senha**: Deve atender aos critérios de segurança
- **Confirmar senha**: Validação da senha escolhida
- **Termos de uso e política de privacidade**: Aceite obrigatório

---

# Configurações do Sistema RDI-KD

![image](https://github.com/user-attachments/assets/92473cb8-d7f2-468f-9ea9-e88f7fa4e007)

## Visão Geral

A página de **Configurações** permite gerenciar suas configurações de conta e preferências pessoais do sistema RDI-KD. Acesse através do menu principal ou diretamente pela URL de configurações.

### Navegação
- **Voltar ao Dashboard**: Botão no canto superior direito para retornar à tela principal

---

## 1. Token do GitHub

### Descrição
Configure seu token de acesso pessoal do GitHub para acessar repositórios privados e realizar análises de código mais abrangentes.

### Configuração do Token

#### Token de Acesso Pessoal
- **Campo de entrada**: Insira seu Personal Access Token (PAT) do GitHub
- **Formato**: `ghp_xxxxxxxxxxxxxxxxxxxx`
- **Máscara de segurança**: O token é automaticamente ocultado por questões de segurança

#### Ações Disponíveis
- **"Criar novo token no GitHub"**: Link direto para criar um novo PAT na plataforma GitHub
- **Botão "Salvar Token"**: Confirma e armazena o token configurado

### Como Criar um Token GitHub
1. Acesse GitHub.com → Settings → Developer settings
2. Clique em "Personal access tokens" → "Tokens (classic)"
3. Gere um novo token com as permissões necessárias:
   - `repo` (acesso completo a repositórios)
   - `read:org` (leitura de organizações)
   - `workflow` (acesso a GitHub Actions)

---

## 2. Configurações de Tema

### Personalização da Interface
Personalize a aparência da interface conforme sua preferência visual.

#### Seleção de Tema
- **Tema atual**: Exibe o tema atualmente ativo
- **Opções disponíveis**:
  - **Tema Escuro**: Interface com fundo escuro (padrão)
  - **Tema Claro**: Interface com fundo claro
- **Ícone de alternância**: Permite trocar entre os temas rapidamente

#### Benefícios por Tema
**Tema Escuro:**
- Reduz o cansaço visual em sessões prolongadas
- Economiza bateria em telas OLED
- Ideal para ambientes com pouca iluminação

**Tema Claro:**
- Melhor legibilidade em ambientes bem iluminados
- Contraste otimizado para leitura de código
- Interface mais tradicional

---

## 3. Alterar Senha

### Segurança da Conta
Mantenha sua conta segura alterando sua senha regularmente.

#### Processo de Alteração
1. **Senha Atual**: Digite sua senha atual para validação
2. **Nova Senha**: Insira a nova senha desejada
3. **Confirmar Nova Senha**: Redigite a nova senha para confirmação
4. **Botão "Alterar Senha"**: Executa a alteração

#### Requisitos de Senha
- Mínimo de 8 caracteres
- Combinação de letras maiúsculas e minúsculas
- Pelo menos um número
- Caracteres especiais recomendados
- Diferente das últimas 3 senhas utilizadas

#### Segurança Adicional
- **Máscaras de entrada**: Todos os campos de senha são ocultados automaticamente
- **Validação em tempo real**: Verificação da força da senha durante a digitação
- **Confirmação obrigatória**: Prevenção contra erros de digitação

---

## 4. Ações da Conta

### Gerenciamento de Sessão
Controle suas sessões e acesso à conta.

#### Sair da Conta
- **Função**: Desconecte-se de sua sessão atual
- **Botão "Sair da Conta"**: Executa o logout de forma segura

---

# Dashboard Principal - RDI-KD

![image](https://github.com/user-attachments/assets/70edc52a-b897-44ae-9ef7-76f8bddedc5f)

![image](https://github.com/user-attachments/assets/d27e1bb1-51f3-45a9-946d-5d5cf0bd1046)

## Visão Geral

O **Dashboard** é a tela principal do sistema RDI-KD, oferecendo uma visão completa e centralizada de toda sua atividade de desenvolvimento. Esta interface fornece métricas importantes, acesso rápido aos repositórios e informações sobre o progresso dos projetos.

---

## 1. Métricas Principais

### Cards de Estatísticas Gerais

#### Total de Repositórios
- **Valor atual**: 15 repositórios
- **Tendência**: +2 novos este mês
- **Ícone**: Símbolo de repositório
- **Indicador de crescimento**: Verde (positivo)

#### Total de Commits
- **Valor atual**: 324 commits
- **Tendência**: +23 esta semana
- **Ícone**: Símbolo de commit/branch
- **Indicador de atividade**: Mostra produtividade recente

#### Colaboradores
- **Valor atual**: 8 colaboradores
- **Tendência**: +1 novo colaborador
- **Ícone**: Símbolo de pessoas/usuários
- **Indicador de crescimento**: Expansão da equipe

#### Projetos Ativos
- **Valor atual**: 12 projetos
- **Tendência**: 3 atualizados hoje
- **Ícone**: Símbolo de gráfico/trending
- **Status de atividade**: Projetos com desenvolvimento ativo

---

## 2. Seção de Repositórios

### Navegação entre Abas
- **Repositórios**: Lista completa dos repositórios do usuário
- **Atividade Recente**: Histórico de ações realizadas recentemente

### Botão de Ação Principal
- **"Novo Repositório"**: Criar um novo repositório diretamente da interface

### Lista de Repositórios

#### 1. projeto-web-app
- **Descrição**: Aplicação web moderna com React e TypeScript
- **Linguagem principal**: TypeScript
- **Estatísticas**:
  - ⭐ 24 stars
  - 🔄 8 forks
- **Última atividade**: 2 horas atrás
- **Ação**: Botão "Ver Repositório"

#### 2. api-backend
- **Status**: Privado
- **Descrição**: API REST para gerenciamento de dados
- **Linguagem principal**: Node.js
- **Estatísticas**:
  - ⭐ 12 stars
  - 🔄 3 forks
- **Última atividade**: 1 dia atrás
- **Ação**: Botão "Ver Repositório"

#### 3. mobile-app
- **Status**: Arquivado
- **Descrição**: Aplicativo mobile híbrido
- **Linguagem principal**: React Native
- **Estatísticas**:
  - ⭐ 6 stars
  - 🔄 2 forks
- **Última atividade**: 3 dias atrás
- **Ação**: Botão "Ver Repositório"

---

## 3. Painel de Ações Rápidas

### Funcionalidades de Acesso Rápido

#### Criar Repositório
- **Função**: Criar novo repositório GitHub
- **Ícone**: Símbolo de adição (+)
- **Acesso direto**: Sem necessidade de navegar para outras páginas

#### Criar Branch
- **Função**: Criar nova branch em repositório existente
- **Ícone**: Símbolo de ramificação
- **Workflow**: Desenvolvimento colaborativo

#### Convidar Colaborador
- **Função**: Adicionar novos membros à equipe
- **Ícone**: Símbolo de pessoas
- **Gestão de equipe**: Facilita expansão do time

#### Configurações
- **Função**: Acesso direto às configurações do sistema
- **Ícone**: Símbolo de engrenagem
- **Link**: Redireciona para página de configurações

---

## 4. Progresso Semanal

### Monitoramento de Atividade
Acompanhe sua produtividade através de métricas semanais com barras de progresso visuais.

#### Commits
- **Meta semanal**: 30 commits
- **Progresso atual**: 23/30 (77%)
- **Status**: Em bom andamento
- **Barra de progresso**: Azul, quase completa

#### Pull Requests
- **Meta semanal**: 8 pull requests
- **Progresso atual**: 5/8 (63%)
- **Status**: Moderado
- **Barra de progresso**: Azul, parcialmente preenchida

#### Issues Fechadas
- **Meta semanal**: 15 issues
- **Progresso atual**: 12/15 (80%)
- **Status**: Próximo da meta
- **Barra de progresso**: Azul, quase completa

### Análise de Performance
- **Tendência**: Atividade consistente durante a semana
- **Pontos fortes**: Alto número de commits e resolução de issues
- **Área de melhoria**: Aumentar número de pull requests

---

## 5. Linguagens Populares

### Distribuição de Tecnologias
Visualização das linguagens mais utilizadas nos seus projetos.

#### TypeScript
- **Porcentagem**: 45%
- **Status**: Linguagem predominante
- **Indicador visual**: Círculo azul

#### JavaScript
- **Porcentagem**: 30%
- **Status**: Segunda mais utilizada
- **Indicador visual**: Círculo amarelo

#### Node.js
- **Porcentagem**: 15%
- **Status**: Backend principal
- **Indicador visual**: Círculo verde

#### React Native
- **Porcentagem**: 10%
- **Status**: Desenvolvimento mobile
- **Indicador visual**: Círculo azul claro

### Insights Tecnológicos
- **Stack principal**: Frontend moderno com TypeScript/React
- **Backend**: Predominantemente Node.js
- **Mobile**: Foco em React Native para desenvolvimento híbrido
- **Tendência**: Forte adoção de TypeScript para type safety

---

## 6. Funcionalidades do Dashboard

### Atualização em Tempo Real
- **Métricas dinâmicas**: Dados atualizados automaticamente
- **Sincronização GitHub**: Integração contínua com repositórios
- **Indicadores visuais**: Status de tendência em tempo real

### Navegação Intuitiva
- **Cards interativos**: Clique para detalhes específicos
- **Ações contextuais**: Botões relevantes para cada repositório
- **Acesso rápido**: Shortcuts para funcionalidades principais

### Personalização
- **Métricas relevantes**: Foco nas informações mais importantes
- **Layout responsivo**: Adaptação a diferentes tamanhos de tela
- **Tema consistente**: Interface integrada com configurações globais

---

## 7. Casos de Uso do Dashboard

### Para Desenvolvedores Individuais
- **Monitoramento**: Acompanhar produtividade pessoal
- **Organização**: Visualizar todos os projetos em um local
- **Planejamento**: Identificar áreas que precisam de atenção

### Para Líderes de Equipe
- **Overview**: Visão geral da atividade da equipe
- **Gestão**: Acompanhar colaboradores e projetos ativos
- **Métricas**: Avaliar performance e produtividade

### Para Gerentes de Projeto
- **Status**: Estado atual de todos os projetos
- **Progresso**: Acompanhamento de metas semanais
- **Recursos**: Distribuição de tecnologias e linguagens

---

### Benefícios Principais
- **Visibilidade completa**: Todos os dados importantes em uma tela
- **Produtividade**: Acesso rápido às ações mais comuns
- **Insights**: Análise visual do progresso e performance
- **Integração**: Conexão seamless com GitHub

### Recomendações de Uso
1. **Consulta diária**: Use como ponto de partida para trabalho
2. **Acompanhamento**: Monitore métricas semanais regularmente
3. **Planejamento**: Use insights para definir próximos passos
4. **Colaboração**: Utilize ações rápidas para gestão de equipe

# Evolução da Inteligência Artificial - RDI-KD

![image](https://github.com/user-attachments/assets/f0771159-357d-4d6d-8346-ca048e77542b)

## Visão Geral

A seção **Evolução da Inteligência Artificial** oferece um dashboard completo para acompanhar o progresso e métricas de desenvolvimento dos modelos de IA integrados ao sistema RDI-KD. Esta interface permite monitorar performance, deployments, treinamentos e análises detalhadas dos algoritmos em uso.

**Descrição**: Acompanhe o progresso e métricas de desenvolvimento dos modelos de I.A.

---

## 1. Métricas Principais

### Cards de Estatísticas Gerais

![image](https://github.com/user-attachments/assets/f0771159-357d-4d6d-8346-ca048e77542b)

#### Modelos Ativos
- **Valor atual**: 24 modelos
- **Tendência**: +3 novos este mês
- **Ícone**: Símbolo de informação
- **Status**: Crescimento positivo na base de modelos

#### Projetos em Desenvolvimento
- **Valor atual**: 8 projetos
- **Tendência**: +2 iniciados recentemente
- **Ícone**: Símbolo de código/desenvolvimento
- **Status**: Atividade de desenvolvimento crescente

#### Precisão Média
- **Valor atual**: 95.2%
- **Tendência**: +2.3% vs mês anterior
- **Ícone**: Símbolo de alvo/precisão
- **Status**: Excelente performance com melhoria contínua

#### Uptime dos Sistemas
- **Valor atual**: 99.8%
- **Status**: Excelente estabilidade
- **Ícone**: Símbolo de tendência/uptime
- **Qualidade**: Alta disponibilidade dos serviços

---

## 2. Navegação por Abas

### Estrutura de Navegação
- **Performance**: Métricas de desempenho e evolução temporal
- **Modelos**: Análise de deployments e versões
- **Treinamento**: Progresso de datasets e validação

---

## 3. Aba Performance

![image](https://github.com/user-attachments/assets/f0771159-357d-4d6d-8346-ca048e77542b)

### Evolução da Performance
**Descrição**: Métricas de precisão, velocidade e eficiência ao longo do tempo

#### Gráfico de Linha Temporal
- **Período**: Janeiro a Junho
- **Eixo Y**: Escala de 0 a 200
- **Duas métricas principais**:
  - **Linha roxa**: Evolução crescente (aprox. 120 a 190)
  - **Linha azul**: Estabilidade (aprox. 80 a 95)

#### Análise de Tendências
- **Crescimento consistente**: Linha roxa mostra melhoria contínua
- **Estabilidade**: Linha azul mantém performance constante
- **Sazonalidade**: Picos de performance em determinados períodos

---

## 4. Uso de Algoritmos

![image5](image5)

### Distribuição de Tecnologias IA

#### Gráfico de Pizza - Algoritmos Utilizados
- **Machine Learning**: 35% (azul)
- **Deep Learning**: 28% (roxo)
- **Natural Language**: 25% (verde)
- **Neural Networks**: 22% (azul claro)

#### Insights Tecnológicos
- **Predominância**: Machine Learning como tecnologia principal
- **Diversificação**: Boa distribuição entre diferentes abordagens
- **Balanceamento**: Uso equilibrado de tecnologias complementares

---

## 5. Atividades Recentes

![image5](image5) ![image6](image6)

### Timeline de Atividades

#### Modelo v2.1 deployado
- **Status**: ✅ Concluído
- **Tempo**: 2 horas atrás
- **Tipo**: Deploy de produção

#### Treinamento de dataset concluído
- **Status**: 📊 Concluído
- **Tempo**: 4 horas atrás
- **Tipo**: Processamento de dados

#### Otimização de performance iniciada
- **Status**: ⚠️ Em andamento
- **Tempo**: 6 horas atrás
- **Tipo**: Melhoria de sistema

#### Precisão aumentou 2.3%
- **Status**: 📈 Melhoria
- **Tempo**: 1 dia atrás
- **Tipo**: Evolução de performance

---

## 6. Ações Rápidas

![image6](image6)

### Funcionalidades de Acesso Direto

#### Novo Modelo
- **Função**: Criar/configurar novo modelo de IA
- **Ícone**: Símbolo de informação
- **Workflow**: Iniciar desenvolvimento de modelo

#### Carregar Dataset
- **Função**: Upload de novos conjuntos de dados
- **Ícone**: Símbolo de documento
- **Processo**: Preparação para treinamento

#### Iniciar Treinamento
- **Função**: Começar processo de treinamento
- **Ícone**: Símbolo de raio/energia
- **Operação**: Execução de algoritmos de aprendizado

#### Relatório Detalhado
- **Função**: Gerar análise completa de performance
- **Ícone**: Símbolo de gráfico
- **Output**: Documento com métricas detalhadas

---

## 7. Aba Modelos

![image7](image7)

### Deployments por Versão
**Descrição**: Número de deployments e taxa de sucesso por versão do modelo

#### Gráfico de Barras Empilhadas
- **Versões analisadas**: v1.0, v1.1, v1.2, v2.0, v2.1
- **Métricas por versão**:
  - **Barras azuis**: Deployments (falhas)
  - **Barras verdes**: Sucesso

#### Análise de Versões
- **v1.0**: ~15 deployments, ~85 sucessos
- **v1.1**: ~20 deployments, ~90 sucessos
- **v1.2**: ~25 deployments, ~95 sucessos
- **v2.0**: ~30 deployments, ~95 sucessos
- **v2.1**: ~28 deployments, ~97 sucessos

#### Tooltip Detalhado (v2.1)
- **Deployments**: 28
- **Success**: 97
- **Taxa de sucesso**: 97/125 = 77.6%

---

## 8. Aba Treinamento

![image8](image8)

### Progresso do Treinamento
**Descrição**: Datasets processados e resultados de treinamento/validação

#### Gráfico de Área Empilhada
- **Período**: Semana 1 a Semana 4
- **Métricas empilhadas**:
  - **Verde**: Treinamento (base)
  - **Laranja**: Validação (topo)

#### Dados da Semana 4
- **Treinamento**: 94 datasets processados
- **Validação**: 98 datasets validados
- **Total**: 192 datasets processados

#### Tendências de Treinamento
- **Crescimento linear**: Aumento consistente ao longo das semanas
- **Validação crescente**: Mais datasets sendo validados
- **Qualidade**: Proporção balanceada entre treinamento e validação

---

## 9. Funcionalidades Avançadas

### Monitoramento em Tempo Real
- **Métricas dinâmicas**: Atualizações automáticas de performance
- **Alertas**: Notificações de mudanças significativas
- **Histórico**: Rastreamento de evolução temporal

### Análise Comparativa
- **Versões**: Comparação entre diferentes versões de modelos
- **Algoritmos**: Análise de performance entre tecnologias
- **Períodos**: Comparação temporal de métricas

### Integração com Desenvolvimento
- **CI/CD**: Integração com pipelines de deployment
- **Versionamento**: Controle de versões de modelos
- **Rollback**: Capacidade de reverter para versões anteriores

---

## 10. Casos de Uso

### Para Data Scientists
- **Experimentação**: Acompanhar resultados de experimentos
- **Otimização**: Identificar oportunidades de melhoria
- **Validação**: Verificar qualidade dos modelos

### Para DevOps/MLOps
- **Deployment**: Monitorar deployments e sua taxa de sucesso
- **Infraestrutura**: Acompanhar uptime e estabilidade
- **Automação**: Integrar com pipelines de CI/CD

### Para Gestores de Produto
- **KPIs**: Acompanhar métricas de negócio
- **Roadmap**: Planejar evoluções dos modelos
- **ROI**: Avaliar retorno dos investimentos em IA

---

## Considerações Finais

O dashboard de **Evolução da Inteligência Artificial** oferece:

### Benefícios Principais
- **Visibilidade completa**: Todas as métricas de IA em um local
- **Decisões baseadas em dados**: Insights para melhorias
- **Monitoramento contínuo**: Acompanhamento em tempo real
- **Gestão de qualidade**: Controle de performance dos modelos

### Melhores Práticas
1. **Monitoramento regular**: Verificar métricas diariamente
2. **Análise de tendências**: Identificar padrões de longo prazo
3. **Validação contínua**: Manter qualidade dos datasets
4. **Deployment controlado**: Usar métricas para decisões de release

## Considerações Finais

O **RDI-KD** é um assistente inteligente para desenvolvedores que buscam agilidade e qualidade em revisões de código. Ele atua como um revisor técnico, apontando falhas, sugerindo melhorias e reforçando boas práticas de desenvolvimento.

 
> **Links Úteis**:
> - [Protótipos vs Wireframes](https://www.nngroup.com/videos/prototypes-vs-wireframes-ux-projects/)
>- Ferramentas:
>> - [Pencil](https://pencil.evolus.vn/)
>> - [MarvelApp](https://marvelapp.com/)
>> - [Figma](https://www.figma.com/)



