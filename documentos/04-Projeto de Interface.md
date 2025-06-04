
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

## Considerações Finais

O **RDI-KD** é um assistente inteligente para desenvolvedores que buscam agilidade e qualidade em revisões de código. Ele atua como um revisor técnico, apontando falhas, sugerindo melhorias e reforçando boas práticas de desenvolvimento.

 
> **Links Úteis**:
> - [Protótipos vs Wireframes](https://www.nngroup.com/videos/prototypes-vs-wireframes-ux-projects/)
>- Ferramentas:
>> - [Pencil](https://pencil.evolus.vn/)
>> - [MarvelApp](https://marvelapp.com/)
>> - [Figma](https://www.figma.com/)



