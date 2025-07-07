# Azure-speech-e-language

Este repositório documenta as atividades realizadas durante o laboratório da plataforma **DIO (Digital Innovation One)**, com foco no uso dos serviços **Azure Speech Studio** e **Language Studio**. O objetivo foi colocar em prática os conhecimentos adquiridos sobre inteligência artificial aplicada à fala e linguagem natural.

## 🧠 Objetivo do Desafio

Explorar ferramentas da Microsoft Azure voltadas para análise de fala (Speech) e linguagem (Language), compreendendo suas funcionalidades e aplicando-as em testes práticos para reforçar o aprendizado.

---

## 🛠️ Tecnologias Utilizadas

- Microsoft Azure
  - Azure Speech Studio
  - Azure Language Studio
- Recursos utilizados:
  - Serviço de Speech (Text-to-Speech e Speech-to-Text)
  - Serviço de Language (Text Analytics - Sentiment Analysis & Opinion Mining)
- Plataforma DIO para orientação do desafio

---

## 📌 Etapas Realizadas

### 1. Criação dos Grupos de Recursos no Azure

- Grupo `idiomal` (para Language Studio)
- Grupo `textofala` (para Speech Studio)

📷 *Captura de tela disponível na pasta `/images`.*

---

### 2. Teste no Language Studio (Sentiment Analysis)

Utilizamos a funcionalidade **Sentiment Analysis com Opinion Mining** para analisar a seguinte avaliação de um hotel:

```txt
Tired hotel with poor service. The Royal Hotel, London, United Kingdom.
This is an old hotel (has been around since 1950's) and the room furnishings are average - becoming a bit old now and require changing.
The internet didn't work and had to come to one of their office rooms to check in for my flight home. The website says it's close to the British Museum, but it's too far to walk.
```

#### 🧪 Resultado:

- **Sentimento geral do documento**: Negativo (100%)
- **Opiniões extraídas**:
  - `hotel`: "tired" (99% negativo)
  - `service`: "poor" (99% negativo)
  - `internet`: "didn't work" (100% negativo)
  - Trecho sobre a localização teve sentimento **neutro**

📷 *Capturas de tela dos resultados também estão incluídas na pasta `/images`.*

---

### 3. Teste no Speech Studio (Conversão de Fala em Texto)

Foi realizado o teste de **conversão de um áudio `.mp3`** com versículo bíblico em inglês:

📁 Áudio: `Psalms 51_10 - Bible Verse of the Day.mp3`

#### 🎧 Resultado:

Transcrição correta do trecho:
```txt
Psalm 51:10. Create in me a clean heart, O God, and renew a steadfast spirit within me.
```

📷 *Captura de tela incluída com resultado da transcrição.*

---

## 🗂️ Estrutura do Repositório

```
/
├── README.md
├── salmo.mp3
├── projeto.txt
└── images/
    ├── print_language_studio_1.jpg
    ├── print_language_studio_2.jpg
    ├── print_speech_studio.jpg
    └── ...
```

---

## 📚 Referências

- [Documentação Speech Studio](https://learn.microsoft.com/en-us/azure/cognitive-services/speech-service/)
- [Documentação Language Studio](https://learn.microsoft.com/en-us/azure/cognitive-services/language-service/)
- [Plataforma DIO](https://www.dio.me)

---

## ✅ Conclusão

Este desafio foi essencial para consolidar os conhecimentos sobre os serviços de IA da Microsoft voltados à linguagem natural. Os testes permitiram observar na prática como a análise de sentimentos e a conversão de fala funcionam, além de reforçar o uso do Azure como plataforma robusta de desenvolvimento de soluções em nuvem.

---

**Desenvolvido por:** César Augusto Fernandes  
 Bootcamp Análise de Dados - Plataforma DIO 🚀
