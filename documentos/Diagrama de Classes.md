# Modelo Relacional – SQL Server

## Tabela: Usuarios
| Campo           | Tipo             | Descrição                         |
|-----------------|------------------|-----------------------------------|
| id_usuario      | INT PRIMARY KEY IDENTITY(1,1) | Identificador único do usuário    |
| nome            | VARCHAR(100)     | Nome do usuário                   |
| email           | VARCHAR(150)     | Email do usuário                  |
| perfil          | VARCHAR(50)      | Perfil (Desenvolvedor, Suporte…) |

---

## Tabela: Commits
| Campo           | Tipo             | Descrição                                |
|-----------------|------------------|------------------------------------------|
| id_commit       | INT PRIMARY KEY IDENTITY(1,1) | ID único do commit                       |
| hash_commit     | VARCHAR(100)     | Hash do commit                           |
| autor           | VARCHAR(100)     | Nome do autor                            |
| mensagem        | TEXT             | Mensagem de commit                       |
| data_commit     | DATETIME         | Data do commit                           |
| id_usuario      | INT FOREIGN KEY  | FK para `Usuarios`                       |

---

## Tabela: Trechos_Codigo
| Campo             | Tipo             | Descrição                              |
|-------------------|------------------|----------------------------------------|
| id_trecho         | INT PRIMARY KEY IDENTITY(1,1) | ID do trecho de código                 |
| id_commit         | INT FOREIGN KEY  | FK para `Commits`                      |
| caminho_arquivo   | VARCHAR(255)     | Caminho do arquivo no repositório      |
| codigo            | TEXT             | Código fonte                           |
| comentario        | TEXT             | Comentários no código                  |
| embedding_vector  | NVARCHAR(MAX)    | Embedding serializado (ex: JSON)       |

> Observação: `embedding_vector` será usado apenas para rastreabilidade. As buscas vetoriais acontecerão fora do SQL Server (Faiss, Elasticsearch etc.)

---

## Tabela: Incidentes
| Campo              | Tipo             | Descrição                              |
|--------------------|------------------|----------------------------------------|
| id_incidente       | INT PRIMARY KEY IDENTITY(1,1) | ID do incidente                        |
| titulo             | VARCHAR(255)     | Título descritivo                      |
| descricao          | TEXT             | Descrição do incidente                 |
| data_criacao       | DATETIME         | Quando foi registrado                  |
| origem             | VARCHAR(50)      | Plataforma (Jira, Zendesk etc.)        |
| id_usuario         | INT FOREIGN KEY  | FK para `Usuarios`                     |

---

## Tabela: Feedbacks
| Campo             | Tipo              | Descrição                           |
|-------------------|-------------------|-------------------------------------|
| id_feedback       | INT PRIMARY KEY IDENTITY(1,1) | ID do feedback                      |
| id_usuario        | INT FOREIGN KEY   | FK para `Usuarios`                  |
| id_trecho         | INT FOREIGN KEY   | FK para `Trechos_Codigo`           |
| util              | BIT               | Usuário achou útil? (1 = sim)       |
| comentario_extra  | TEXT              | Comentários do usuário              |
| data_feedback     | DATETIME          | Data de registro do feedback        |

---

## Tabela: Consultas
| Campo             | Tipo              | Descrição                          |
|-------------------|-------------------|------------------------------------|
| id_consulta       | INT PRIMARY KEY IDENTITY(1,1) | ID da consulta feita               |
| id_usuario        | INT FOREIGN KEY   | FK para `Usuarios`                 |
| texto_pergunta    | TEXT              | Pergunta feita pelo usuário        |
| data_consulta     | DATETIME          | Data da consulta                   |
