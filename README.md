# Projeto_Integrador_HoneyDukes

#### Termo de Abertura de Projeto(TAP)

## Controle de Versões
| Versão | Data | Autor | Nota da Revisão |
|:---|:---:|---:| ---: |
| 1.0 | 02/06/2026 | Allan de Sousa Almeida | |

### Stack Tecnológica
| Camada | Tecnologia |
| :--- | :--- |
| **Back-end** | Node.js / Knex.js / Postman / JavaScript |
| **Banco de dados** | MySQL |
| **Front-end** | HTML5 / CSS3 / JavaScript (Vanilla - Sem Frameworks) |
| **Hospedagem / Deploy** | Railway (Back-end) / Vercel (Front-end) |
| **Documentação / Protótipo**| Swagger (API) / Figma (UI/UX) / GitHub (Repositório Central) |


### Objetivos deste Projeto
Desenvolver em equipe uma plataforma de e-commerce (loja virtual) temática para a doceria **Honeyduke's**, integrando o planejamento de projetos, construção de interface responsiva, regras de negócio no back-end e modelagem completa de banco de dados para simular uma operação real de vendas online.

### Justificativa do Projeto
Consolidar de forma prática e integrada os conhecimentos adquiridos nas disciplinas de Projetos, Banco de Dados, Backend e Frontend. O projeto justifica-se pela necessidade de criar uma aplicação completa com API própria funcional e persistência de dados, preparando a equipe para os desafios reais do mercado de desenvolvimento web.

## Critérios de Aceite da API (Rotas RESTful)
| EndPoint | Critério |
| :--- | :--- |
| `POST /produtos` | Cria um novo doce. Retorna status `201 Created` e persiste o registro no banco de dados. |
| `GET /produtos` | Lista os doces. Retorna status `200 OK` com a listagem completa ou filtros por categoria. |
| `GET /produtos/:id` | Busca detalhada. Retorna status `200 OK` com os detalhes do produto correto baseado no ID. |
| `PUT /produtos/:id` | Atualiza um doce. Retorna status `200 OK` e altera as informações persistidas no banco. |
| `DELETE /produtos/:id` | Remove um doce. Retorna status `200 OK` ou `204 No Content` e deleta o registro do banco. |

### Descrição do Projeto e Principais Requisitos
* #### Descrição Geral
  O projeto consiste em um site de e-commerce responsivo para a doceria temática **Honeyduke's**. A plataforma contará com uma área pública para os clientes navegarem e uma área administrativa exclusiva para os gerentes do sistema operarem o CRUD dos produtos.
* #### Módulos e Requisitos do Escopo Mínimo:
  * **Landing Page:** Página inicial responsiva, atrativa e com a identidade visual da Honeyduke's.
  * **Catálogo de Produtos:** Exibição dinâmica de produtos consumidos diretamente do banco de dados.
  * **Organização por Categorias:** Filtros e divisões estruturadas dos produtos da loja.
  * **Página de Detalhes:** Tela focada na exibição das informações completas, preços e especificações de um doce selecionado.
  * **Área Administrativa:** Painel administrativo protegido para operações de inserção, edição e exclusão de produtos e categorias (CRUD).
  * **Integração Frontend + Backend:** Interface consumindo a API REST desenvolvida pelo grupo.
  * **Persistência de Dados:** Banco de dados MySQL modelado e populado corretamente.
  * **Regra de Participação:** Todos os integrantes da equipe devem atuar ativamente em todas as quatro frentes do projeto (Projetos, Front, Back e Banco).

### Equipe do Projeto
|Nome| Função |
| :--- | :--- |
| Allan Almeida | Full-stack |
| Maxwillian Santana | Back-End |
| Bryan Alves | DBA |
| Thiago Costa | Front-End |
| Pedro Rodrigues | DBA |
| Prof° Yuri Komuta | P.O / Gerente do Projeto |
| Prof° Marcel Teixeira | Staff Back-End |
| Prof° Fernando Leonid | Staff Front-End |
| Prof° Joao Meyer | Staff Banco de Dados |



#### Gerente do Projeto: 
 Yuri Komuta

#### Patrocinador:
SENAI Prof° Vicente Amato

### Premissas e Restrições
* **Premissa 01:** O frontend deve ser construído puramente com HTML, CSS e JavaScript Vanilla, sendo proibida a utilização de frameworks (como React, Vue ou Angular).
* **Premissa 02:** O repositório centralizador do GitHub deve conter um README detalhado com os links de deploy e o vídeo pitch.
* **Restrição 01:** O prazo final para entrega do sistema completamente integrado é o dia **19/06/2026**.
* **Restrição 02:** Prevenção contra quedas do sistema configurando corretamente o tratamento de erros na API e hospedagem confiável.

### Entregáveis
| Classificação | Item / EndPoint | Tipo / Descrição | Método HTTP |
| :--- | :--- | :--- | :--- |
| **API** | `/produtos` | CREATE (Cadastro de Doces) | POST |
| **API** | `/produtos` | READ (Listagem / Detalhes) | GET |
| **API** | `/produtos/:id` | UPDATE (Edição de dados) | PUT |
| **API** | `/produtos/:id` | DELETE (Exclusão de registros) | DELETE |
| **Documentação** | TAP | Termo de Abertura de Projeto | N/A |
| **Documentação** | Swagger | Documentação interativa das rotas da API | N/A |
| **Documentação** | Modelagem BD | Arquivos dos modelos Conceitual, Lógico e Físico | N/A |
| **Design** | Protótipo Figma | Telas estáticas e fluxo navegável da aplicação | N/A |
| **Código** | Repositórios Git | Códigos-fonte estruturados no GitHub | N/A |
| **Mídia** | Vídeo Pitch | Apresentação em vídeo do projeto (Máx. 5 minutos) | N/A |


#### Marcos (Cronograma de Sprints)
| Marcos / Sprints | Data da Entrega | Entregáveis Principais |
| :--- | :---: | :--- |
| **Sprint 01** | 09/06/2026 | Requisitos funcionais/não funcionais, Protótipo estático no Figma e Modelagem de Banco (Conceitual e Lógico). |
| **Sprint 02** | 11/06/2026 | Documentação das rotas no Swagger, Protótipo navegável no Figma, Criação dos repositórios no GitHub e Script do Modelo Físico do Banco. |
| **Sprint 03** | 19/06/2026 | Desenvolvimento e finalização do Frontend e Backend, Integração total do sistema e entrega do Repositório Centralizador com os links e Vídeo Pitch. |

### Riscos
1. **Gargalo na Integração Final (Sprint 3):** Risco de incompatibilidade entre os dados enviados pelo Frontend e recebidos pelo Backend por falta de comunicação prévia sobre o contrato da API.
2. **Complexidade no JS Puro:** Possível atraso no desenvolvimento da reatividade e componentes do Frontend devido à restrição de não usar frameworks estruturados.
3. **Problemas de Versionamento (Conflitos no Git):** Risco de perda de código ou atrasos nas entregas por falta de sincronia e falta de domínio em resoluções de *merge conflicts* nos repositórios.
4. **Curto Espaço de Tempo entre as Sprints:** O intervalo de apenas 2 dias entre a Sprint 1 e a Sprint 2 exige agilidade extrema para não acumular demandas para a entrega final.
