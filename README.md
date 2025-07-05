# Azure Speech & Language Studio - Documentação Técnica

Este repositório contém uma documentação técnica e prática sobre o uso das ferramentas **Microsoft Azure Speech Studio** e **Language Studio**, com foco em aplicações reais de **análise de fala** e **processamento de linguagem natural (NLP)**.

📌 Ideal para analistas e cientistas de dados, desenvolvedores e equipes de produto que buscam integrar recursos de fala e linguagem natural em suas aplicações.

---

## 📘 Sumário

- [Objetivo]
- [Visão Geral das Ferramentas]
- [Casos de Uso]
- [Speech Studio]
  - [Transcrição de Áudio]
  - [Reconhecimento de Fala Personalizado]
  - [Conversão Texto-para-Fala]
- [Language Studio]
  - [Análise de Sentimentos]
  - [Extração de Entidades Nomeadas
  - [Classificação de Texto]
- [Arquitetura de Integração]
- [Boas Práticas]
- [Requisitos]
- [Como Usar]
- [Referências]

---

## 🎯 Objetivo

Este projeto tem como objetivo apresentar uma abordagem prática para o uso de serviços de fala e linguagem natural oferecidos pela Azure, aplicados em cenários reais como:

- Atendimento automatizado
- Análise de feedbacks de clientes
- Geração automática de legendas
- Monitoramento de sentimentos em ligações de call center
- Enriquecimento de dados com análise semântica

---

## 🛠️ Visão Geral das Ferramentas

### Azure Speech Studio

Ferramenta baseada na nuvem para transcrição automática, conversão de texto em fala e personalização de modelos de fala.

### Azure Language Studio

Plataforma para análise de texto com funcionalidades como análise de sentimentos, extração de entidades, classificação de tópicos e mais.

---

## 💡 Casos de Uso

| Ferramenta        | Aplicação                                                                 |
|-------------------|---------------------------------------------------------------------------|
| Speech Studio      | Transcrição de reuniões e chamadas, comandos por voz, acessibilidade      |
| Language Studio    | Análise de e-mails, reviews, chats, formulários de NPS e SAC               |
| Integração Speech + Language | Conversão de fala para texto seguida de análise de sentimentos ou tópicos |

---

## 🗣️ Speech Studio

### 📌 Transcrição de Áudio

- Suporte a arquivos `.wav`, `.mp3`, `.ogg`, etc.
- Idiomas e dialetos customizáveis

### 📌 Reconhecimento de Fala Personalizado

- Criação de modelos acústicos personalizados
- Adaptação a vocabulários específicos do domínio (ex: medicina, jurídico)

### 📌 Conversão Texto-para-Fala (TTS)

- Geração de vozes realistas com Neural TTS
- Suporte a SSML para entonação e pausa

---

## 🧠 Language Studio

### 📌 Análise de Sentimentos

- Identificação de polaridade (positivo, neutro, negativo)
- Análise por sentença e por documento

### 📌 Extração de Entidades Nomeadas (NER)

- Padrões como nomes, locais, datas, produtos
- Entidades personalizadas via treinamento

### 📌 Classificação de Texto

- Multiclasse ou multilabel
- Treinamento supervisionado com datasets próprios

---

## 🧩 Arquitetura de Integração

```mermaid
graph LR
A[Entrada de Áudio/Texto] --> B[Speech Studio - Transcrição]
B --> C[Language Studio - NLP]
C --> D[Dashboard/Aplicativo/Análise]

