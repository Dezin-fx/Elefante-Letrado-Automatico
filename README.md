# 📘 Elefante Letrado Automático

![Status](https://img.shields.io/badge/status-active-brightgreen)
![Platform](https://img.shields.io/badge/platform-browser-blue)
![Type](https://img.shields.io/badge/type-userscript-yellow)

## 📌 Sobre o projeto

O Elefante Letrado Automático é um Script para Tampermonkey que adiciona recursos de automação e assistência dentro da plataforma Elefante Letrado.

O Script fornece ferramentas para automatizar a navegação, detectar atividades e, opcionalmente, utilizar modelos de Inteligência Artificial para auxiliar na interpretação e resolução de quizzes.

## 🔒 É seguro?

- O script roda apenas no seu navegador  
- Nenhum dado é enviado para Servidores proprios
- Quando a IA está ativada, apenas o conteúdo necessário para análise das perguntas é enviado diretamente para a API escolhida pelo usuário
- A chave da API é armazenada localmente pelo Tampermonkey

## Principais funções:

- Navegação automática entre páginas.
- Sistema de auto-paginação.
- Detecção automática de quizzes.
- Extração automática de perguntas e alternativas.
- Integração opcional com IA através do OpenRouter.
- Interface gráfica integrada à página.
- Configuração inicial diretamente pela interface do script.
- Detecção automática do livro.
- Modo sem IA para utilização apenas dos recursos de automação.

## Instalação e Uso

O script pode ser usado com Tampermonkey (recomendado)

### 1. Instalar Tampermonkey
- Chrome / Firefox / Edge: extensão oficial

### 2. Adicionar o script
- Abra o painel do Tampermonkey.
- Criar novo Script
- Colar o conteúdo do `Script.js`
- Salvar Script

### 3. Acessar a plataforma
- Abrir o Elefante Letrado normalmente

# Atenção❗

## Variáveis

O script utiliza o [Config.js](https://github.com/Dezin-fx/Elefante-Letrado-Automatico/blob/main/Config.js) para declarar o valor das variáveis usadas. Para usar o script é necessário alterar os valores de `OPENROUTER_KEY` `BOOK_TITLE` e `BOOK_CONTEXT`

>`OPENROUTER_KEY` É a chave API, o que conecta a IA no script. Por questões de privacidade, é necessário o usuario criar a própria API KEY para usar o sistema automatizado com IA. Tutorial em: **🔑 API utilizada**
>
> `BOOK_CONTEXT` É do que se trata o livro, colocar gênero, autor(a), etc. Recomendo fortemente ir no chatGPT ou na IA de sua preferência e pedir um resumo completo do livro pra colocar aqui; pois assim a IA do script ganha mais contexto!
> 
> `BOOK_TITLE` Apenas o titulo do livro.

## 🔑 API utilizada

O projeto utiliza a API da [OpenRouter](https://openrouter.ai)

### É necessário:

* Criar uma conta no OpenRouter
* Gerar uma API key em [OpenRouter Key](https://openrouter.ai/workspaces/default/keys)
* Inserir no arquivo Config.js em `OPENROUTER_KEY`

#### O script depende de um campo de contexto onde o usuário informa o conteúdo base do livro ou atividade atual. Esse contexto é usado como referência para interpretar perguntas e gerar respostas mais coerentes.
