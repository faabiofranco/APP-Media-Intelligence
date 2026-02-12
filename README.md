# 📡 APP Media Intelligence

Ferramenta de **Inteligência de Mídia** com análise por IA para profissionais de comunicação.  
Faça perguntas em linguagem natural sobre sua cobertura de mídia e obtenha gráficos, análises e ações estratégicas.

---

## 🚀 Deploy no GitHub Pages (passo a passo)

### 1. Criar o repositório

1. Acesse [github.com](https://github.com) e faça login
2. Clique em **"New repository"**
3. Nome sugerido: `media-intelligence`
4. Marque como **Public** (obrigatório para GitHub Pages grátis)
5. Clique em **"Create repository"**

### 2. Fazer upload do arquivo

**Opção A — pelo navegador (mais fácil):**
1. No repositório criado, clique em **"Add file" → "Upload files"**
2. Arraste o arquivo `index.html` para a área de upload
3. Clique em **"Commit changes"**

**Opção B — pelo Git:**
```bash
git clone https://github.com/SEU_USUARIO/media-intelligence.git
cd media-intelligence
cp /caminho/para/index.html .
git add index.html
git commit -m "Initial deploy"
git push
```

### 3. Ativar o GitHub Pages

1. No repositório, clique em **"Settings"** (aba)
2. No menu lateral, clique em **"Pages"**
3. Em **"Source"**, selecione: `Deploy from a branch`
4. Em **"Branch"**, selecione: `main` e pasta `/ (root)`
5. Clique em **"Save"**

### 4. Acessar o APP

Após 1-2 minutos, seu app estará disponível em:
```
https://SEU_USUARIO.github.io/media-intelligence/
```

---

## 🔑 Configurar API Keys

Com o app rodando no GitHub Pages (HTTPS), todas as APIs funcionam.  
Clique em **🔑 API Keys** no app e insira sua chave:

| LLM | Onde obter | Modelo usado |
|-----|-----------|--------------|
| **OpenAI** | [platform.openai.com/api-keys](https://platform.openai.com/api-keys) | gpt-4o-mini |
| **DeepSeek** | [platform.deepseek.com](https://platform.deepseek.com/api_keys) | deepseek-chat |
| **Claude** | [console.anthropic.com](https://console.anthropic.com/settings/keys) | claude-sonnet-4-5 |
| **Grok** | [console.x.ai](https://console.x.ai) | grok-3-mini |
| **Qwen** | [dashscope.aliyuncs.com](https://dashscope.aliyuncs.com) | qwen-plus |

> ⚠️ As chaves são salvas apenas no `localStorage` do seu navegador. Nunca são enviadas para outros servidores além da API escolhida.

---

## 📊 Funcionalidades

- **Upload Excel/CSV** — Importa planilhas de clipping classificado
- **Dashboard** — KPIs + 5 gráficos automáticos (sentimento, RPS, mídias, temporal, protagonismo)
- **Chat IA** — Perguntas em linguagem natural com gráficos e insights estratégicos
- **Base de Dados** — Tabela com busca em tempo real

### Análises disponíveis no Chat

| Pergunta | O que retorna |
|----------|--------------|
| *"Sentimento do Bradesco"* | Positivo/negativo por player + gráfico |
| *"RPS por player"* | Ranking de qualidade midiática |
| *"AVE total"* | Equivalência publicitária por player |
| *"Evolução temporal"* | Linha do tempo da cobertura |
| *"Top veículos"* | Ranking por volume de publicações |
| *"Protagonismo"* | % de notícias onde a marca é protagonista |
| *"Temas abordados"* | Ranking de assuntos mais cobertos |
| *"Porta-vozes"* | Executivos mais citados |
| *"Motivação das notícias"* | Espontânea / Proativa / Reativa |
| *"Distribuição por Tier"* | Tier 1 / 2 / 3 por player |
| *"Resumo geral"* | Overview executivo completo |

---

## 📋 Campos da planilha suportados

`Id` · `Titulo` · `Midia` · `Conteudo` · `UrlOriginal` · `DataVeiculacao` · `Veiculo` · `Secao` · `Jornalistas` · `Canais` · `EquivalenciaPublicitaria` · `ClassificacaoVeiculo` · `Impacto` · `VeiculoCidade` · `VeiculoEstado` · `Player` · `Motivação` · `Espaço` · `Ocorrências` · `Personagens` · `Porta_Voz` · `Temas` · `Relevância` · `Protagonismo` · `Sentimento` · `RPS` · `RPS Potencial` · `RPS Eficaz`

---

## 🛡️ Modos de operação

| Modo | Quando | Funcionalidades |
|------|--------|----------------|
| **Análise Local** | Sempre (sem API Key) | 12 tipos de análise pré-programadas, offline |
| **LLM Real** | GitHub Pages + API Key | Qualquer pergunta em linguagem livre + análise inteligente |

---

## ⚙️ Tecnologias

- HTML5 + CSS3 + JavaScript (vanilla) — sem frameworks, sem build
- [Chart.js 4.4](https://www.chartjs.org/) — gráficos
- [SheetJS (xlsx)](https://sheetjs.com/) — leitura de Excel
- Google Fonts: Syne + DM Sans

---

*Desenvolvido para equipes de Assessoria de Imprensa e Inteligência de Mídia.*
