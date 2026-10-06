<!-- 🔮 BANNER DO PERFIL -->

<p align="center">
  <img src="https://i.pinimg.com/1200x/9f/db/bd/9fdbbd8988b4a9f999ef70e78232bed0.jpg" style="border-radius: 12px;" />
</p>

<h1 align="center">👋 Olá! Eu sou o Gabriel Kenzo</h1>

<p align="center">
  Desenvolvedor Júnior • Python • IA & Automação • Dados & BI
</p>

---

## 🧑‍💻 Sobre mim

🎓 Formado em **Análise e Desenvolvimento de Sistemas**
📊 Pós-graduado em **Big Data Analytics & Business Intelligence**
💻 Desenvolvo com **Python**, integrando **APIs, LLMs e serviços externos** para automatizar processos
🤖 Já construí **bots, pipelines com LLM e sistemas de alertas automáticos**
🛠️ Mais de 5 anos de experiência prática com **suporte técnico, troubleshooting, hardware e redes**
🚀 Aprendo construindo: pego um problema real, transformo em projeto e documento o que aprendi.

Hoje meu foco é **desenvolvimento, inteligência artificial e automação**, evoluindo tanto na parte técnica quanto na construção de soluções completas.

---

## 🤖 O que eu já fiz com IA

* **Integração com LLMs via API** (Groq / LLaMA 3.3 70B), com system prompt e user prompt
* **Prompt Engineering:** testes de personalidade, tom e comportamento do modelo
* **Structured Output:** modelo instruído a responder em JSON, processado pelo código
* **Lógica de decisão sobre a resposta do modelo:** o sistema lê o resultado do LLM e escolhe o próximo passo do pipeline (base de uma abordagem agêntica)
* **Geração de áudio (TTS)** com ElevenLabs e mixagem com ffmpeg
* **IA dentro de um bot:** o modelo devolve tags internas que o código interpreta para atualizar o estado do jogo (HP, inimigos, turnos)
* **API própria em Flask** para expor um pipeline de IA em uma interface web local

---

## 🛠️ Competências

### 💻 Desenvolvimento & Automação

![Python](https://img.shields.io/badge/Python-20232A?style=for-the-badge&logo=python&logoColor=3776AB)
![Flask](https://img.shields.io/badge/Flask-20232A?style=for-the-badge&logo=flask&logoColor=white)
![JSON](https://img.shields.io/badge/JSON-20232A?style=for-the-badge&logo=json&logoColor=white)
![Git](https://img.shields.io/badge/Git-20232A?style=for-the-badge&logo=git&logoColor=F05032)
![GitHub](https://img.shields.io/badge/GitHub-20232A?style=for-the-badge&logo=github&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-20232A?style=for-the-badge&logo=githubactions&logoColor=2088FF)

### 🤖 IA & Integrações

![LLMs](https://img.shields.io/badge/LLMs-20232A?style=for-the-badge&logo=openai&logoColor=white)
![Prompt Engineering](https://img.shields.io/badge/Prompt_Engineering-20232A?style=for-the-badge&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-20232A?style=for-the-badge&logoColor=white)
![ElevenLabs](https://img.shields.io/badge/ElevenLabs-20232A?style=for-the-badge&logo=elevenlabs&logoColor=white)
![ffmpeg](https://img.shields.io/badge/ffmpeg-20232A?style=for-the-badge&logo=ffmpeg&logoColor=007808)
![REST APIs](https://img.shields.io/badge/REST_APIs-20232A?style=for-the-badge&logo=fastapi&logoColor=009688)
![Telegram](https://img.shields.io/badge/Telegram_Bot_API-20232A?style=for-the-badge&logo=telegram&logoColor=26A5E4)
![Discord](https://img.shields.io/badge/Discord_API-20232A?style=for-the-badge&logo=discord&logoColor=5865F2)

### 📊 Dados & BI (base da pós-graduação)

![SQL](https://img.shields.io/badge/SQL-20232A?style=for-the-badge&logo=postgresql&logoColor=4169E1)
![Pandas](https://img.shields.io/badge/Pandas-20232A?style=for-the-badge&logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-20232A?style=for-the-badge&logo=powerbi&logoColor=F2C811)
![Spark](https://img.shields.io/badge/Spark-20232A?style=for-the-badge&logo=apachespark&logoColor=E25A1C)
![scikit-learn](https://img.shields.io/badge/scikit--learn-20232A?style=for-the-badge&logo=scikitlearn&logoColor=F7931E)

### 🖥️ TI & Suporte

![Windows](https://img.shields.io/badge/Windows-20232A?style=for-the-badge&logo=windows&logoColor=0078D6)
![Hardware](https://img.shields.io/badge/Hardware-20232A?style=for-the-badge&logo=pcgamingwiki&logoColor=white)
![Redes](https://img.shields.io/badge/Redes_(DHCP_/_DNS)-20232A?style=for-the-badge&logoColor=white)

---

## 🚀 Projetos

### ✈️ K-Finder — Monitor automático de passagens aéreas

Sistema que monitora preços de voos e avisa quando aparece uma oferta dentro do critério definido pelo usuário.

* Usuário configura **rotas e preço máximo** por um bot do **Telegram**
* **GitHub Actions** executa as buscas automaticamente a cada 6h, sem depender do meu PC
* Dados de voos do Google Flights via **Apify**, com filtro por faixa de preço
* **Histórico de preços** para evitar alertas repetidos
* Alertas por **Telegram** e **e-mail em HTML** com link direto para o Google Flights
* Suporte a múltiplas rotas, múltiplos usuários e múltiplos destinatários
* Credenciais protegidas com **GitHub Secrets** (após uma exposição acidental no histórico do Git, rotacionei todas as chaves)

`Python` `Apify` `Telegram Bot API` `SMTP` `GitHub Actions`

🔗 [Ver repositório](https://github.com/KenzoWaka10/k-finder)

---

### 🎙️ Laboratório de IA — Pipeline de LLM, decisão automática e áudio

Projeto experimental para entender, na prática, como integrar LLMs a aplicações reais.

```text
Texto (.txt) → LLM analisa → JSON estruturado → sistema decide a voz
            → ElevenLabs gera o áudio → ffmpeg mistura → MP3 final
```

* LLM retorna **clima, intensidade, emoção principal e narração** em JSON
* O código usa a resposta do modelo para **tomar decisões** no pipeline
* **API Flask** (`POST /processar`) e interface web local com player de áudio

`Python` `Groq` `LLaMA 3.3 70B` `ElevenLabs` `Flask` `ffmpeg`

📌 Repositório em preparação.

---

### 🎲 BotGM — Mestre de RPG com IA para Discord

Bot que narra campanhas de RPG usando LLM e controla turnos, personagens e combate.

* Comandos como `!iniciar`, `!acao`, `!roll`, `!status`, `!turnos`
* A IA devolve **tags internas** (ex.: HP e inimigos) que o código interpreta para atualizar o estado sem mostrá-las ao jogador
* **Memória persistente** da campanha, controle de HP e vínculo entre usuário do Discord e personagem
* Migração do provedor de IA para a **Groq** por questão de custo

`Python` `discord.py` `Groq` `LLaMA 3.3 70B` `Git/GitHub`

> Projeto iniciado por outra pessoa e abandonado. Eu assumi a continuidade: corrigi problemas, refiz partes e implementei novas funcionalidades. Não sou o criador original.

---

## 📚 Atualmente estudando e reforçando

```text
Python
├── APIs e boas práticas de desenvolvimento
├── Automação (incluindo n8n)
└── Refazer meus projetos do zero para consolidar o aprendizado

Inteligência Artificial
├── Agentes de IA
├── RAG e embeddings
├── MCP
└── Integração de ferramentas

Dados & BI
├── Análise de dados
├── Business Intelligence
└── Visualização de dados
```

---

## 📈 GitHub

<p align="center">
  <img width="48%" src="https://github-readme-stats.vercel.app/api?username=KenzoWaka10&show_icons=true&theme=tokyonight&hide_border=true" />
  <img width="48%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=KenzoWaka10&layout=compact&theme=tokyonight&hide_border=true" />
</p>

---

## 🎯 Objetivo

Busco uma oportunidade na área de **Tecnologia**, especialmente em posições relacionadas a:

**Desenvolvimento • Python • IA • Automação • Dados • BI**

Meu objetivo é continuar evoluindo através de projetos práticos, contribuindo com soluções reais e construindo uma base cada vez mais sólida em tecnologia.

---

## 🌐 Onde me encontrar

📎 **LinkedIn:** [linkedin.com/in/gabriel-kenzo-5b86a52a9](https://www.linkedin.com/in/gabriel-kenzo-5b86a52a9/)

📧 **E-mail:** [kenzowakassugui7@gmail.com](mailto:kenzowakassugui7@gmail.com)

💻 **GitHub:** [github.com/KenzoWaka10](https://github.com/KenzoWaka10)

---

<p align="center">
  <i>Construindo, aprendendo e evoluindo um projeto de cada vez. 🚀</i>
</p>
