# 📸 python-gpt-scheduler

**⚠️ Atenção: Este projeto está em desenvolvimento (WIP). ⚠️**

## 🎯 Sobre o Projeto

O **python-gpt-scheduler** é um assistente inteligente para transformar anotações de caderno em lembretes agendados.

O objetivo é criar uma aplicação que permita ao usuário tirar uma foto de suas anotações manuscritas. Uma IA (provavelmente uma LLM via API, como GPT ou Gemini) irá então "ler" a foto, identificar qualquer tarefa associada a uma data e, automaticamente, agendar um lembrete por e-mail para o dia correto.

O principal desafio deste projeto é explorar a viabilidade de construir essa solução ponta-a-ponta **usando primariamente o ecossistema Python** ao invés do android studio + kotlin, incluindo a interface do usuário no celular (provavelmente usarei Kivy ou BeeWare).

### O Fluxo de Trabalho 

1.  **Captura:** O usuário abre o app no celular e tira uma foto de suas anotações.
2.  **Processamento:** A imagem é enviada para um backend Python.
3.  **Análise (IA):** O backend usa uma API de IA (OCR + LLM) para extrair o texto da imagem e identificar padrões como "Medir vidro no cliente tal - 28/10" ou "Comprar massa para vidro na próxima sexta".
4.  **Agendamento:** O sistema interpreta a data e agenda uma tarefa.
5.  **Notificação:** No dia marcado, um serviço de backend envia um e-mail de lembrete para o usuário.

## 💻 Tecnologias (Potenciais)

* **Linguagem:** Python 3
* **App Framework (A definir):** Kivy ou BeeWare 
* **IA (LLM + OCR):** OpenAI API ou Google Gemini API.
* **Agendador de Tarefas (A definir):** APScheduler ou Celery com Redis (mais robusto).
* **Banco de Dados:** SQLite.
  
## 🚀 Como Executar o Projeto (Em breve)
