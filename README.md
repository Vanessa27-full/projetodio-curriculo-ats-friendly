## # 💼 CareerFlow — Matchmaking de Vagas + Currículo ATS Friendly

![Lovable](https://img.shields.io/badge/Lovable-FF4F64?style=for-the-badge)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge\&logo=react\&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge\&logo=typescript\&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge\&logo=tailwindcss\&logoColor=white)
![ShadCN UI](https://img.shields.io/badge/ShadCN_UI-000000?style=for-the-badge\&logo=shadcnui\&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge\&logo=supabase\&logoColor=white)
![Vibe Coding](https://img.shields.io/badge/Vibe_Coding-AI-8B5CF6?style=for-the-badge)

Aplicação web desenvolvida como projeto de **Vibe Coding para a DIO**, utilizando Inteligência Artificial e o **Lovable** para transformar requisitos escritos em uma solução funcional.

O **CareerFlow** ajuda candidatos a analisar vagas de emprego, comparar requisitos com o próprio perfil profissional, identificar lacunas de conhecimento e gerar versões personalizadas de currículo com foco em compatibilidade com sistemas **ATS — Applicant Tracking System**.

---

## 🚀 Demonstração

🔗 **Aplicação:** https://career-compass-359.lovable.app/

---

## 🎯 Objetivo

Durante processos seletivos, muitas pessoas utilizam o mesmo currículo para diferentes vagas, mesmo quando cada oportunidade possui requisitos, tecnologias e palavras-chave específicas.

O CareerFlow foi criado para tornar esse processo mais estratégico.

A aplicação permite responder perguntas como:

* Meu perfil combina com esta vaga?
* Quais requisitos eu já possuo?
* Quais competências estão faltando?
* Quais palavras-chave são importantes?
* Meu currículo está adequado para esta oportunidade?
* Qual versão do currículo devo enviar?

O fluxo principal do produto é:

```text
PERFIL PROFISSIONAL
        ↓
       VAGA
        ↓
      MATCH
        ↓
    SKILL GAP
        ↓
CURRÍCULO PERSONALIZADO
        ↓
    ATS SCORE
        ↓
   CANDIDATURA
        ↓
    ANALYTICS
```

---

## ✨ Principais Funcionalidades

### 👤 Perfil Profissional

Cadastro estruturado de informações como:

* dados profissionais;
* objetivo de carreira;
* experiências;
* formação acadêmica;
* Hard Skills;
* Soft Skills;
* projetos;
* cursos;
* certificações;
* idiomas;
* LinkedIn;
* GitHub;
* portfólio.

O perfil funciona como a **fonte principal de verdade da aplicação**.

---

### 💼 Análise de Vagas

O usuário pode adicionar uma vaga e informar sua descrição completa.

O sistema identifica informações como:

* cargo;
* empresa;
* senioridade;
* modalidade;
* localização;
* requisitos obrigatórios;
* requisitos desejáveis;
* diferenciais;
* tecnologias;
* idiomas;
* responsabilidades;
* palavras-chave relevantes.

As informações extraídas podem ser revisadas pelo usuário.

---

### 🎯 Matchmaking de Vagas

O CareerFlow compara:

> **Perfil Profissional × Vaga**

e gera um **Match Score de 0 a 100**.

| Match   | Classificação |
| ------- | ------------- |
| 90–100% | Excelente     |
| 75–89%  | Muito bom     |
| 60–74%  | Bom           |
| 40–59%  | Moderado      |
| 0–39%   | Baixo         |

O cálculo considera diferentes fatores:

| Critério                 | Peso |
| ------------------------ | ---: |
| Skills técnicas          |  30% |
| Experiência              |  20% |
| Senioridade              |  15% |
| Formação                 |  10% |
| Ferramentas              |  10% |
| Idiomas                  |   5% |
| Localização / Modalidade |   5% |
| Palavras-chave           |   5% |

A análise não depende apenas de correspondências literais.

O sistema também considera equivalências como:

```text
JS → JavaScript
TS → TypeScript
React.js → React
Node → Node.js
Postgres → PostgreSQL
```

---

### 🔎 Match Explicável

Além da porcentagem, o usuário consegue visualizar como a pontuação foi formada.

Exemplo:

```text
Match: 82%

Skills              26/30
Experiência          13/20
Senioridade          12/15
Formação             10/10
Ferramentas           8/10
Idiomas               4/5
Modalidade            5/5
Keywords              4/5
```

Também são apresentados:

```text
Você possui

✓ React
✓ JavaScript
✓ Git
✓ REST API
```

e:

```text
Requisitos ausentes

Docker
AWS
Jest
```

---

## 📚 Skill Gap

O módulo de **Skill Gap** analisa as vagas cadastradas e identifica tecnologias ou competências recorrentes que ainda não aparecem no perfil profissional.

Exemplo:

```text
Docker
Encontrado em 11 vagas

AWS
Encontrado em 9 vagas

Jest
Encontrado em 7 vagas
```

A ideia é utilizar essas informações como apoio para definir novos estudos.

O sistema não recomenda adicionar habilidades inexistentes ao currículo.

---

## 📄 Currículo ATS Friendly

O usuário pode manter um currículo principal e gerar versões específicas para diferentes oportunidades.

Fluxo:

```text
PERFIL
↓
VAGA
↓
REQUISITOS
↓
PALAVRAS-CHAVE
↓
SELEÇÃO DE CONTEÚDO
↓
CURRÍCULO PERSONALIZADO
```

A aplicação pode:

* reorganizar informações;
* melhorar a escrita;
* destacar experiências relevantes;
* priorizar habilidades;
* adaptar o resumo profissional;
* melhorar bullet points.

Sempre utilizando informações já existentes no perfil.

---

## 🤖 ATS Score

Além do Match, a aplicação calcula um indicador separado:

> **Currículo × Vaga**

Esse indicador é chamado de **ATS Score**.

Exemplo:

```text
ATS Score

89/100
```

A análise pode considerar:

```text
Keywords             27/30
Skills               23/25
Experiência          19/25
Estrutura            10/10
Formação              5/5
Legibilidade          5/5
```

O ATS Score é apresentado como uma **estimativa de compatibilidade**, e não como garantia de aprovação.

---

## 🧠 Match x ATS Score

Os dois indicadores possuem objetivos diferentes.

### Match

Analisa:

```text
PERFIL × VAGA
```

Responde:

> Meu perfil profissional combina com esta oportunidade?

### ATS Score

Analisa:

```text
CURRÍCULO × VAGA
```

Responde:

> Este currículo está bem direcionado para esta oportunidade?

---

## 📝 Editor de Currículo

O aplicativo possui um editor com visualização do documento.

No desktop:

```text
EDITOR                    PREVIEW

Resumo                    Currículo A4
Experiência
Habilidades
Formação
Projetos
```

No mobile:

```text
Editar | Visualizar | ATS
```

O usuário pode:

* editar textos;
* reorganizar seções;
* ativar ou desativar seções;
* reorganizar experiências;
* revisar sugestões;
* acompanhar o ATS Score;
* visualizar o documento;
* salvar alterações.

---

## 📥 Exportação

O currículo pode ser exportado em:

* PDF.

Estrutura pensada para ser ATS Friendly:

* uma coluna;
* títulos tradicionais;
* texto selecionável;
* tipografia legível;
* estrutura simples;
* sem gráficos desnecessários;
* sem barras de habilidades;
* sem elementos decorativos que prejudiquem a leitura automática.

---

## 🗂️ Gestão de Candidaturas

Após analisar uma vaga e criar o currículo, o usuário pode acompanhar o processo seletivo.

O CareerFlow utiliza uma visualização em Kanban:

```text
Interessada
↓
Salva
↓
Currículo criado
↓
Candidatura enviada
↓
Triagem
↓
Entrevista RH
↓
Entrevista técnica
↓
Proposta
↓
Contratada
```

Candidaturas encerradas também podem ser registradas.

---

## 🕐 Timeline

Cada candidatura pode possuir um histórico.

Exemplo:

```text
10 Ago
Candidatura enviada

12 Ago
Recrutador entrou em contato

14 Ago
Entrevista RH

18 Ago
Entrevista técnica
```

---

## 📊 Analytics

O aplicativo possui uma área dedicada ao acompanhamento da busca por emprego.

Indicadores planejados:

* vagas analisadas;
* Match médio;
* ATS Score médio;
* currículos criados;
* candidaturas enviadas;
* entrevistas;
* propostas;
* taxa de resposta.

Também podem ser apresentados:

* candidaturas por período;
* candidaturas por status;
* evolução do Match;
* evolução do ATS;
* habilidades mais solicitadas;
* funil de candidaturas.

---

## 🛡️ Integridade das Informações

Um dos principais requisitos do projeto é impedir que a IA invente informações para aumentar artificialmente o Match ou ATS Score.

A IA **não deve inventar**:

* experiências;
* empresas;
* habilidades;
* formação;
* certificações;
* cursos;
* projetos;
* idiomas;
* métricas;
* datas;
* anos de experiência.

Exemplo:

Se uma vaga exigir:

```text
Docker
```

e Docker não estiver cadastrado no perfil:

```text
Docker é solicitado nesta vaga, mas não consta no seu perfil profissional.
```

A aplicação não deverá adicionar essa tecnologia automaticamente ao currículo.

> **Otimizar um currículo não significa falsificar informações.**

---

## 🎨 Design System

O projeto utiliza:

### ShadCN UI

como Design System principal.

A interface foi planejada para ser:

* moderna;
* minimalista;
* profissional;
* responsiva;
* acessível;
* semelhante a um produto SaaS.

### 🌙 Tema Escuro

```text
Preto + Vermelho
```

O vermelho é utilizado principalmente em:

* CTAs;
* ações principais;
* elementos selecionados;
* indicadores;
* navegação ativa.

### ☀️ Tema Claro

```text
Branco + Azul Escuro
```

O azul escuro é utilizado para:

* ações principais;
* navegação;
* indicadores;
* elementos selecionados.

---

## 📱 Responsividade

A experiência foi planejada para:

* desktop;
* notebook;
* tablet;
* smartphone.

Adaptações para mobile incluem:

```text
Sidebar → Drawer / Sheet

Tabelas → Cards

Kanban → Scroll horizontal

Editor → Tabs
```

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia        | Utilização                       |
| ----------------- | -------------------------------- |
| **Lovable**       | Desenvolvimento por Vibe Coding  |
| **React**         | Interface da aplicação           |
| **TypeScript**    | Tipagem e estrutura do projeto   |
| **Tailwind CSS**  | Estilização                      |
| **ShadCN UI**     | Design System                    |
| **Lucide Icons**  | Iconografia                      |
| **Supabase**      | Persistência e banco de dados    |
| **IA Generativa** | Análise e otimização de conteúdo |

---

## 🧩 Arquitetura Conceitual

Principais entidades da aplicação:

```text
profiles
experiences
educations
skills
profile_skills
projects
courses
certifications
languages

jobs
job_requirements
job_keywords

job_matches
match_details

resumes
resume_versions
ats_analyses

applications
application_events
application_notes

app_preferences
```

O perfil profissional funciona como base para todas as análises.

```text
PROFILE
   ↓
 JOBS
   ↓
 MATCHES
   ↓
 RESUMES
   ↓
 ATS
   ↓
 APPLICATIONS
```

---

## 🔐 Primeira Versão sem Autenticação

Para reduzir a fricção durante a validação do MVP, a primeira versão foi planejada sem:

* login;
* cadastro;
* OAuth;
* logout;
* recuperação de senha.

O fluxo é:

```text
ENTRAR
↓
USAR
```

A arquitetura poderá receber autenticação futuramente.

---

## 🧪 Testes e Validação

Durante os testes da aplicação, os principais fluxos previstos para o MVP foram validados com sucesso. A criação e edição do perfil profissional funcionaram corretamente, assim como o cadastro de vagas e a interpretação automática das descrições. A identificação de requisitos, o cálculo do Match, a explicação da compatibilidade e a análise de Skill Gaps também apresentaram o comportamento esperado.

A geração de currículos personalizados, o cálculo do ATS Score e a edição dos currículos foram testados e funcionaram conforme planejado. O fluxo de criação de candidaturas e a alteração de status também foram validados com sucesso.

Além disso, o Dashboard apresentou os dados corretamente, assim como a área de Analytics. A responsividade da aplicação foi testada em diferentes tamanhos de tela, e a alternância entre os temas claro e escuro também funcionou adequadamente.

Como pontos ainda pendentes, a página de **Analytics** apresenta funcionalidades que precisam de ajustes adicionais em alguns cenários, e a página de **Configurações** ainda não está funcionando corretamente. Esses itens permanecem como pontos de melhoria para as próximas versões do projeto. **Erro 404 Page not found
The page you're looking for doesn't exist or has been moved.**

De forma geral, o fluxo principal do CareerFlow está funcional, permitindo ao usuário criar seu perfil, cadastrar e analisar vagas, visualizar o Match, identificar Skill Gaps, gerar currículos personalizados, consultar o ATS Score e acompanhar candidaturas.

---

## ⚠️ Limitações

Como a solução utiliza Inteligência Artificial para interpretar textos, alguns resultados podem exigir revisão.

Exemplos:

* requisitos ambíguos;
* tecnologias com nomes diferentes;
* descrição incompleta da vaga;
* classificação incorreta entre requisito obrigatório e desejável;
* interpretação semântica;
* extração de informações de currículos.

Por isso, o usuário deve poder revisar informações importantes antes de utilizá-las.

Além disso:

> O Match Score e o ATS Score são indicadores estimados e não representam garantia de contratação ou aprovação em sistemas ATS.

---

## 📸 Screenshots

```markdown
<img width="1920" height="1030" alt="Dashboard — Matchmaking de vagas e currículo ATS -" src="https://github.com/user-attachments/assets/43c41dbe-ea1b-45bc-91d0-77e871f80e2d" />

<img width="1920" height="1030" alt="Vagas — Matchmaking de vagas e currículo ATS - " src="https://github.com/user-attachments/assets/856fb07d-e96d-4496-9de7-3aa9df379c11" />

<img width="1920" height="1030" alt="Match — Matchmaking de vagas e currículo ATS -  src="https://github.com/user-attachments/assets/e7ada89f-826e-4c0f-aa2a-68939cc27b15" />

<img width="1920" height="1030" alt="Currículo  — Matchmaking de vagas e currículo ATS - " src="https://github.com/user-attachments/assets/edfe7a30-7b00-48d8-8ae0-6cc65e6b5ac8" />

<img width="1920" height="1030" alt="Candidatura — Matchmaking de vagas e currículo ATS - " src="https://github.com/user-attachments/assets/25e11eaa-b051-4a2b-aebb-213abd69bbb4" />

<img width="1920" height="1030" alt="Perfil — Matchmaking de vagas e currículo ATS - " src="https://github.com/user-attachments/assets/368515e5-5ed3-481e-8f68-615d3fa1e85b" />

<img width="1920" height="1030" alt="Analystic erro — Matchmaking de vagas e currículo ATS - " src="https://github.com/user-attachments/assets/73e29fcf-b537-48d3-8367-b6fb5ccae448" />

```

---

## 🧠 Aprendizados

O projeto permitiu explorar Vibe Coding além da simples geração de interfaces.

Durante o desenvolvimento foram trabalhados conceitos como:

* levantamento de requisitos;
* criação de PRD;
* regras de negócio;
* UX/UI;
* Design Systems;
* estruturação de dados;
* Inteligência Artificial;
* processamento de linguagem natural;
* Matchmaking;
* análise ATS;
* validação de dados;
* responsividade;
* acessibilidade;
* arquitetura de produto.

Um dos principais aprendizados foi perceber que a qualidade do resultado produzido por uma IA depende diretamente da clareza dos requisitos fornecidos.

Vibe Coding não elimina a necessidade de pensar sobre o produto.

Ele muda a forma como o produto é construído.

---

## 🔮 Roadmap

Possíveis evoluções:

* [ ] Autenticação e criação de contas
* [ ] Sincronização entre dispositivos
* [ ] Importação automática de PDF
* [ ] Importação de DOCX
* [ ] Importação de vaga por URL
* [ ] Integração com APIs de empregos
* [ ] Exportação DOCX
* [ ] Novos templates de currículo
* [ ] Currículo em inglês
* [ ] Notificações
* [ ] Lembretes de follow-up
* [ ] Integração com calendário
* [ ] Histórico avançado de currículos
* [ ] Recomendação de estudos baseada no Skill Gap
* [ ] Comparação de versões de currículo

---

## 📌 Fluxo Principal

```text
CRIAR PERFIL
      ↓
ADICIONAR VAGA
      ↓
ANALISAR VAGA
      ↓
CALCULAR MATCH
      ↓
IDENTIFICAR SKILL GAP
      ↓
GERAR CURRÍCULO
      ↓
CALCULAR ATS
      ↓
EXPORTAR PDF
      ↓
REGISTRAR CANDIDATURA
      ↓
ACOMPANHAR PROCESSO
      ↓
ANALISAR RESULTADOS
```

---

## 💬 Conclusão

O **CareerFlow** demonstra como Inteligência Artificial, Vibe Coding e boas práticas de produto podem ser combinados para resolver um problema real.

A proposta não é apenas gerar currículos.

O objetivo é criar uma jornada completa para ajudar candidatos a compreender melhor as oportunidades, apresentar suas competências de forma estratégica e organizar seus processos seletivos.

O princípio central do projeto é:

> **A IA deve ajudar o candidato a comunicar melhor suas competências reais, e não criar competências que ele não possui.**

---

## 👩‍💻 Autora

**Vanessa Costa Pereira**

Estudante de **Análise e Desenvolvimento de Sistemas e Futura Desenvolvedora F**

Projeto desenvolvido para fins de estudo, portfólio e desafio de **Vibe Coding da DIO**.
