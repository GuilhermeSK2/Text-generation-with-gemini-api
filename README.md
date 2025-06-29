# Geração de Texto com a API Google Gemini

Este projeto é um exemplo prático de como interagir com a API Google Gemini para gerar texto. Ele demonstra a configuração básica para usar o modelo `gemini-2.0-flash` e realizar uma simples troca de mensagens, onde o modelo atua como um assistente que responde de forma clara e objetiva.

## Visão Geral

A API Google Gemini oferece acesso a modelos de linguagem avançados, permitindo uma ampla gama de aplicações, desde geração de conteúdo criativo até assistentes virtuais. Este projeto foca em uma aplicação direta: fornecer um prompt ao modelo e receber uma resposta generativa, simulando uma conversa com um assistente útil e direto.

## Estrutura do Projeto

* `Gemini.ipynb`: O notebook Jupyter que contém todo o código para configurar o acesso à API, instanciar o modelo Gemini e interagir com ele.

## Tecnologias Utilizadas

* **Python 3**
* **Google Generative AI SDK (`google-generativeai`)**: Para interagir com a API Gemini.
* **Jupyter Notebook**: Para execução e demonstração interativa do código.
* **Modelo Gemini**: `gemini-2.0-flash` (um modelo otimizado para tarefas de geração rápida).

## Exemplo de Uso

Você pode modificar a variável `conversation` para interagir com o modelo de diferentes maneiras. Por exemplo:

```python
# Mude a conversa para fazer outras perguntas
conversation = "Qual é a capital do Brasil?"
response = model.generate_content(conversation)
print(response.text.strip())

conversation = "Me dê uma dica para aprender Python."
response = model.generate_content(conversation)
print(response.text.strip())
