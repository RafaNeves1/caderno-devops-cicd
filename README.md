# Caderno Temático: DevOps & CI/CD com NotebookLM

> Projeto prático desenvolvido para o desafio da DIO — explorando Inteligência Artificial como ferramenta de aprendizagem ativa.

---

## Sumário

1. [Contexto e Objetivos](#-contexto-e-objetivos)
2. [Curadoria de Fontes](#-curadoria-de-fontes)
3. [Engenharia de Prompts e Cicatrizes](#-engenharia-de-prompts-e-cicatrizes)
4. [Miniguia de Estudo — Entrega Final](#-miniguia-de-estudo--entrega-final)
   - [Resumos Estruturados](#-resumos-estruturados)
   - [Glossário](#-glossário)
   - [Prompts Reutilizáveis](#-prompts-reutilizáveis)

---

##  Contexto e Objetivos

### Por que DevOps & CI/CD?

DevOps deixou de ser uma tendência para se tornar uma **prática padrão da indústria de software**. Empresas de todos os tamanhos buscam profissionais capazes de integrar desenvolvimento e operações, automatizar pipelines e garantir entregas contínuas com qualidade. Dominar CI/CD (Integração Contínua e Entrega/Deploy Contínuo) é hoje um diferencial competitivo real no mercado.

Este caderno temático foi construído no **NotebookLM** como parte de um processo de estudo ativo, combinando curadoria de fontes confiáveis com engenharia de prompts estruturada.

### Objetivos de Estudo

| # | Objetivo | Status |
|---|----------|--------|
| 1 | Compreender os fundamentos da cultura DevOps e seus princípios | ✅ |
| 2 | Entender o fluxo completo de um pipeline CI/CD | ✅ |
| 3 | Conhecer as principais ferramentas do ecossistema (GitHub Actions, Jenkins, Docker) | ✅ |
| 4 | Aprender boas práticas de automação de testes e deploy | ✅ |
| 5 | Consolidar um vocabulário técnico sólido na área | ✅ |

---

##  Curadoria de Fontes

As fontes abaixo foram selecionadas por serem **abertas, confiáveis e em formato compatível com upload no NotebookLM** (texto/PDF). Priorizei materiais de organizações reconhecidas e documentação oficial.

---

###  Fonte 1 — The DevOps Handbook (resumo público / capítulos abertos)
- **Tipo:** PDF / Artigo
- **Link:** [https://itrevolution.com/product/the-devops-handbook/](https://itrevolution.com/product/the-devops-handbook/)
- **Por que escolhi:** Obra de referência escrita pelos criadores do movimento DevOps. Fornece a base conceitual e histórica da disciplina, os três caminhos (Three Ways) e exemplos reais de transformação organizacional.
- **Conteúdo relevante:** Princípios do fluxo, feedback e aprendizado contínuo.

---

###  Fonte 2 — Documentação Oficial do GitHub Actions
- **Tipo:** Documentação Web (exportável para PDF)
- **Link:** [https://docs.github.com/en/actions](https://docs.github.com/en/actions)
- **Por que escolhi:** GitHub Actions é uma das ferramentas CI/CD mais adotadas no mercado atualmente. A documentação oficial é clara, repleta de exemplos práticos e constantemente atualizada.
- **Conteúdo relevante:** Conceito de workflows, triggers, jobs, steps, runners e marketplace de actions.

---

###  Fonte 3 — Google Cloud: O que é CI/CD?
- **Tipo:** Artigo Web
- **Link:** [https://cloud.google.com/solutions/devops](https://cloud.google.com/solutions/devops)
- **Por que escolhi:** O Google Cloud oferece um guia técnico e imparcial sobre CI/CD, com diagramas de arquitetura e comparativos entre abordagens. Excelente para contextualizar os conceitos em cenários reais de cloud.
- **Conteúdo relevante:** Diferença entre CI, CD (Continuous Delivery) e CD (Continuous Deployment), métricas DORA.

---

###  Fonte 4 — Red Hat: O que é DevOps?
- **Tipo:** Artigo Web
- **Link:** [https://www.redhat.com/pt-br/topics/devops](https://www.redhat.com/pt-br/topics/devops)
- **Por que escolhi:** A Red Hat é referência em open source e DevOps empresarial. O artigo está disponível em português, é denso tecnicamente e aborda desde a cultura até ferramentas como Ansible, OpenShift e Kubernetes.
- **Conteúdo relevante:** Cultura DevOps, integração com containers e orquestração.

---

###  Fonte 5 — Atlassian: CI vs CD vs CD
- **Tipo:** Artigo Web
- **Link:** [https://www.atlassian.com/br/devops/continuous-delivery-tutorials/continuous-integration-vs-delivery-vs-deployment](https://www.atlassian.com/br/devops/continuous-delivery-tutorials/continuous-integration-vs-delivery-vs-deployment)
- **Por que escolhi:** A Atlassian (criadora do Jira e Bitbucket) apresenta de forma didática as diferenças entre Integração Contínua, Entrega Contínua e Deploy Contínuo — conceitos frequentemente confundidos. Disponível em português.
- **Conteúdo relevante:** Distinção clara entre CI / Continuous Delivery / Continuous Deployment com exemplos visuais.

---

##  Engenharia de Prompts e Cicatrizes

Esta seção documenta o processo real de interação com o NotebookLM: as perguntas formuladas, os refinamentos necessários e as lições aprendidas. O mercado valoriza o raciocínio por trás dos resultados!

---

###  Rodada 1 — Prompts de Exploração Inicial

**Objetivo:** Mapear o que as fontes tinham de mais relevante antes de aprofundar.

#### Prompt 1.1
```
Com base nas fontes carregadas, quais são os 5 conceitos mais fundamentais
de DevOps que um desenvolvedor iniciante precisa entender?
```
**Resposta obtida:** O NotebookLM listou: (1) Cultura de colaboração Dev+Ops, (2) Automação de pipelines, (3) Monitoramento contínuo, (4) Infraestrutura como código (IaC) e (5) Feedback loops. Cada item veio com referência a trechos das fontes — o que foi muito útil para validação.

**Dificuldade encontrada:** A resposta foi genérica demais. Precisei reformular para obter profundidade.

---

#### Prompt 1.2 (refinamento)
```
Aprofunde o conceito de "Feedback Loop" em DevOps. Como ele se manifesta
na prática dentro de um pipeline CI/CD? Cite exemplos das fontes.
```
**Resposta obtida:** Desta vez o NotebookLM trouxe exemplos concretos: notificações automáticas de falha de build, gates de qualidade no pipeline, alertas de monitoramento em produção. As citações das fontes foram precisas.

**Lição aprendida:** Prompts específicos com "cite exemplos das fontes" ativam muito melhor o comportamento de RAG do NotebookLM.

---

###  Rodada 2 — Prompts de Comparação e Diferenciação

**Objetivo:** Clarificar conceitos que causam confusão frequente.

#### Prompt 2.1
```
Qual a diferença exata entre Continuous Integration, Continuous Delivery
e Continuous Deployment? Apresente em formato de tabela comparativa.
```
**Resposta obtida:** Tabela clara com 4 colunas: conceito, objetivo, gatilho de execução e quem aprova o avanço. A fonte da Atlassian foi a mais citada aqui.

** Funcionou bem de primeira.** Pedir formato específico (tabela, lista, etc.) melhora muito a organização da resposta.

---

#### Prompt 2.2
```
Entre Jenkins e GitHub Actions, quais as principais diferenças de
arquitetura e casos de uso ideais para cada um? Use as fontes para embasar.
```
**Resposta obtida:** Comparativo interessante, mas o NotebookLM alertou que as fontes carregadas não tinham conteúdo aprofundado sobre Jenkins especificamente. Ele indicou quais afirmações vinham das fontes e quais eram conhecimento geral.

** Cicatriz registrada:** Lacuna nas fontes sobre Jenkins. Solução: incluir a documentação oficial do Jenkins como Fonte 6 em estudos futuros.

---

###  Rodada 3 — Prompts de Síntese e Aplicação Prática

**Objetivo:** Transformar o conhecimento absorvido em material de estudo consolidado.

#### Prompt 3.1
```
Crie um resumo estruturado em tópicos sobre o ciclo completo de um pipeline
CI/CD, desde o commit do desenvolvedor até o deploy em produção.
Inclua as etapas, ferramentas envolvidas e boas práticas de cada fase.
```
**Resposta obtida:** Resumo de alta qualidade com 6 etapas claras. Usou como base principal a documentação do GitHub Actions e o artigo do Google Cloud.

---

#### Prompt 3.2
```
Quais são as métricas DORA e por que elas são importantes para medir a
maturidade de um time DevOps? Explique cada uma com linguagem acessível.
```
**Resposta obtida:** Explicação das 4 métricas (Deployment Frequency, Lead Time for Changes, Change Failure Rate, Time to Restore Service) com linguagem clara. O NotebookLM referenciou o conteúdo do Google Cloud e do DevOps Handbook.

** Dica de ouro:** Adicionar "com linguagem acessível" ou "para um desenvolvedor júnior" calibra bem o nível de profundidade das respostas.

---

#### Prompt 3.3 — O mais difícil
```
Elabore um glossário com os 15 termos mais importantes de DevOps e CI/CD,
com definição técnica objetiva e um exemplo prático de cada um.
```
** Dificuldade encontrada:** Na primeira tentativa, o NotebookLM gerou apenas 10 termos e alguns exemplos ficaram vagos. Precisei iterar:

```
Continue o glossário a partir do termo 11. Para os exemplos, seja mais
específico — mencione um comando, arquivo de configuração ou situação real.
```
** Resultado final:** Glossário completo com 15 termos, exemplos técnicos concretos. A estratégia de quebrar em partes menores funcionou muito bem.

---

## Miniguia de Estudo — Entrega Final

---

### Resumos Estruturados

---

#### Módulo 1 — Fundamentos de DevOps

DevOps é uma **cultura e conjunto de práticas** que une as equipes de Desenvolvimento (Dev) e Operações (Ops) com o objetivo de entregar software com mais velocidade, qualidade e confiabilidade.

Seus pilares fundamentais são os **Três Caminhos (Three Ways)**:

1. **Fluxo (Flow):** Otimizar o movimento do trabalho da esquerda (desenvolvimento) para a direita (produção), eliminando desperdícios e gargalos.
2. **Feedback:** Criar loops de retorno rápidos e contínuos — testes automatizados, monitoramento e alertas — para detectar e corrigir problemas o mais cedo possível.
3. **Aprendizado Contínuo:** Construir uma cultura de experimentação, tolerância a falhas controladas e melhoria iterativa.

A cultura DevOps é tão importante quanto as ferramentas. Sem quebrar os silos organizacionais entre Dev e Ops, nenhuma ferramenta de automação gera o resultado esperado.

---

#### Módulo 2 — CI/CD: Conceitos e Diferenças

Os termos CI e CD são frequentemente confundidos. Veja a distinção exata:

| Conceito | Significado | O que automatiza | Aprovação humana? |
|---|---|---|---|
| **CI** — Continuous Integration | Integração Contínua | Build + testes a cada commit | Não (automático) |
| **CD** — Continuous Delivery | Entrega Contínua | CI + prepara artefato para deploy | **Sim** (deploy é manual) |
| **CD** — Continuous Deployment | Deploy Contínuo | CI + deploy automático em produção | Não (totalmente automático) |

A maioria das empresas adota **Continuous Delivery** como ponto de equilíbrio: automação total até a homologação e aprovação humana para produção.

---

#### Módulo 3 — Anatomia de um Pipeline CI/CD

Um pipeline moderno percorre as seguintes etapas após um `git push`:

```
[1. Source] → [2. Build] → [3. Test] → [4. Security Scan] → [5. Staging Deploy] → [6. Production Deploy]
```

**Detalhamento de cada fase:**

- **Source:** Trigger pelo commit/PR no repositório (GitHub, GitLab, Bitbucket). Controle de versão é a base de tudo.
- **Build:** Compilação do código, instalação de dependências, geração do artefato (binário, imagem Docker, pacote npm etc.).
- **Test:** Execução de testes unitários, de integração e de contrato. Um pipeline sem testes não é um pipeline de qualidade.
- **Security Scan:** Análise estática de código (SAST), verificação de vulnerabilidades em dependências (SCA) e análise de secrets expostos.
- **Staging Deploy:** Deploy em ambiente espelho da produção para testes de aceitação (UAT) e smoke tests.
- **Production Deploy:** Deploy na produção com estratégia de rollout (blue/green, canary, rolling update).

---

#### Módulo 4 — GitHub Actions na Prática

O GitHub Actions é uma plataforma de CI/CD nativa do GitHub, baseada em arquivos YAML dentro da pasta `.github/workflows/`.

**Estrutura básica de um workflow:**

```yaml
# .github/workflows/ci.yml
name: Pipeline CI

on:
  push:
    branches: [main, develop]
  pull_request:
    branches: [main]

jobs:
  build-and-test:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout do código
        uses: actions/checkout@v4

      - name: Configurar Node.js
        uses: actions/setup-node@v4
        with:
          node-version: '20'

      - name: Instalar dependências
        run: npm ci

      - name: Executar testes
        run: npm test

      - name: Build da aplicação
        run: npm run build
```

**Conceitos-chave do GitHub Actions:**
- **Workflow:** Processo automatizado completo, definido em YAML.
- **Trigger (`on`):** Evento que inicia o workflow (push, pull_request, schedule, etc.).
- **Job:** Grupo de steps executados no mesmo runner.
- **Step:** Unidade individual de execução (comando ou action).
- **Runner:** Servidor que executa os jobs (ubuntu-latest, windows-latest, macos-latest ou self-hosted).
- **Action:** Componente reutilizável do Marketplace do GitHub.

---

#### Módulo 5 — Métricas DORA

As métricas **DORA (DevOps Research and Assessment)** são o padrão da indústria para medir a performance de times de engenharia:

| Métrica | O que mede | Elite |
|---|---|---|
| **Deployment Frequency** | Com que frequência o time faz deploy em produção | Múltiplos por dia |
| **Lead Time for Changes** | Tempo do commit até o deploy em produção | < 1 hora |
| **Change Failure Rate** | % de deploys que causam incidentes | 0–15% |
| **Time to Restore Service** | Tempo para recuperar o serviço após uma falha | < 1 hora |

Times que atingem métricas de elite têm **127x mais deploys** e **3x menor taxa de falhas** que times de baixa performance (Google State of DevOps Report).

---

### Glossário

| Termo | Definição Técnica | Exemplo Prático |
|---|---|---|
| **Pipeline** | Sequência automatizada de etapas que transforma código-fonte em software entregue | Um arquivo `ci.yml` no GitHub Actions que executa build → test → deploy |
| **CI (Continuous Integration)** | Prática de integrar código frequentemente com verificações automáticas a cada commit | Ao abrir um PR, testes rodam automaticamente e bloqueiam merge se falharem |
| **CD (Continuous Delivery)** | Extensão do CI que garante o software sempre pronto para deploy, com aprovação manual final | Pipeline que gera um artefato validado e aguarda clique humano para ir à produção |
| **CD (Continuous Deployment)** | Toda mudança que passa nos testes é automaticamente para produção sem intervenção humana | Startup que faz 50 deploys/dia sem aprovação manual |
| **Artifact** | Produto gerado pelo processo de build (binário, imagem Docker, pacote) | Imagem `minha-app:v1.2.3` publicada no Docker Hub |
| **Runner** | Servidor (físico ou virtual) que executa os jobs do pipeline | `ubuntu-latest` no GitHub Actions ou um servidor EC2 self-hosted |
| **IaC (Infrastructure as Code)** | Gerenciamento de infraestrutura por meio de código versionável | Arquivo `main.tf` do Terraform que cria uma VPC na AWS |
| **Docker** | Plataforma de containers que empacota aplicação e dependências em unidades isoladas | `docker build -t minha-app .` cria uma imagem portável |
| **Rollback** | Processo de reverter um deploy problemático para a versão anterior estável | `kubectl rollout undo deployment/minha-app` no Kubernetes |
| **Blue/Green Deployment** | Estratégia com dois ambientes idênticos; tráfego migra do blue para o green gradualmente | Load balancer aponta para o novo ambiente (green) após validação |
| **Canary Release** | Deploy para um subconjunto de usuários antes do rollout completo | 5% dos usuários recebem a nova versão; se estável, expande para 100% |
| **SAST** | Static Application Security Testing — análise de vulnerabilidades no código-fonte | SonarQube identificando SQL Injection no código antes do deploy |
| **Gate de Qualidade** | Critério mínimo que o pipeline exige antes de avançar para a próxima etapa | Cobertura de testes < 80% bloqueia o pipeline automaticamente |
| **Webhook** | Notificação HTTP automática disparada por um evento | GitHub notifica o Jenkins quando um push ocorre no repositório |
| **Self-hosted Runner** | Servidor próprio configurado para executar jobs do CI/CD | Máquina interna da empresa registrada no GitHub para rodar pipelines |

---

### Prompts Reutilizáveis

Coleção de prompts testados e validados para futuras revisões e aprofundamento no tema.

---

#### Categoria: Revisão de Conceitos

```
Explique o conceito de [TERMO] em DevOps como se eu fosse um desenvolvedor
júnior sem experiência com o tema. Use uma analogia do mundo real e
um exemplo técnico concreto.
```

```
Quais são os erros mais comuns que times iniciantes cometem ao implementar
[CI / CD / pipelines / IaC]? Como evitá-los?
```

```
Compare [FERRAMENTA A] e [FERRAMENTA B] em termos de arquitetura, casos de
uso ideais, curva de aprendizado e integração com o ecossistema atual.
```

---

#### Categoria: Aprofundamento Técnico

```
Descreva passo a passo como estruturar um pipeline CI/CD completo para
uma aplicação [Node.js / Python / Java] usando [GitHub Actions / Jenkins /
GitLab CI]. Inclua as etapas de build, test, security scan e deploy.
```

```
Como implementar a estratégia de deploy [blue-green / canary / rolling update]
na prática? Quais ferramentas são necessárias e quais são os trade-offs?
```

```
Quais boas práticas devo seguir ao armazenar secrets e variáveis de ambiente
em um pipeline CI/CD? Cite pelo menos 3 abordagens com exemplos.
```

---

#### Categoria: Síntese e Geração de Material de Estudo

```
Com base nas fontes carregadas, crie um resumo estruturado em tópicos sobre
[TEMA]. Organize por: conceito central → como funciona → boas práticas →
ferramentas mais usadas.
```

```
Gere 10 perguntas de revisão (no estilo de entrevista técnica) sobre [TEMA]
com as respostas esperadas, baseando-se nas fontes disponíveis.
```

```
Elabore um glossário com os [N] termos mais importantes de [TEMA].
Para cada termo inclua: definição técnica objetiva, exemplo prático com
código ou comando real, e por que é importante conhecer.
```

---

#### Categoria: Resolução de Dúvidas Específicas

```
Tenho dúvida sobre a diferença entre [CONCEITO A] e [CONCEITO B].
Explique com clareza, use uma tabela comparativa e dê um exemplo que
ilustre quando usar cada um.
```

```
Preciso configurar [FUNCIONALIDADE] no [GITHUB ACTIONS / JENKINS / GITLAB CI].
Quais são os passos e qual seria o arquivo de configuração mínimo funcional?
```

---

## Como Reproduzir Este Projeto

1. Acesse [NotebookLM](https://notebooklm.google.com/) com sua conta Google
2. Crie um novo notebook com o nome **"DevOps & CI/CD — Caderno Temático"**
3. Faça upload ou adicione os links das 5 fontes listadas na seção [Curadoria de Fontes](#-curadoria-de-fontes)
4. Aguarde o processamento e comece com os **Prompts de Exploração Inicial** da seção de Engenharia de Prompts
5. Evolua para prompts de síntese e use a seção de **Prompts Reutilizáveis** para futuras revisões

---

## Reflexão Final

Este projeto demonstrou que o NotebookLM funciona melhor quando usado com **intencionalidade**:

- Prompts específicos geram respostas melhores que perguntas abertas
- Pedir formato (tabela, tópicos, glossário) organiza o output
- Iterar sobre a resposta com refinamentos é mais eficiente que o prompt perfeito de primeira
- A qualidade do output depende diretamente da qualidade das fontes carregadas
- O NotebookLM é honesto sobre lacunas — aproveite isso para identificar o que falta estudar

---

## Autor

Desenvolvido como parte do **Desafio DIO — Caderno Temático com NotebookLM**

[LinkedIn](www.linkedin.com/in/rafael-neves-748957175)

[GitHub](https://github.com/RafaNeves1)

---

*"A automação não substitui o pensamento crítico — ela o amplifica."*
