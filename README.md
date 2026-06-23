# 📘 Elefante Letrado Automatico

![Status](https://img.shields.io/badge/status-active-brightgreen)
![Platform](https://img.shields.io/badge/platform-browser-blue)
![Type](https://img.shields.io/badge/type-userscript-yellow)

## 📌 Sobre o projeto

Este script automatiza interações na plataforma Elefante Letrado diretamente no navegador.

Ele reduz ações manuais ao detectar atividades, extrair perguntas e gerar respostas automaticamente com auxílio de IA

## As principais funções são:

- Navegação automática entre páginas quando não há interação necessária  
- Detecção de quizzes e perguntas na interface  
- Extração automática de perguntas e alternativas do DOM  
- Geração de respostas utilizando IA (OpenRouter)  
- Uso de contexto do livro para melhorar a precisão das respostas  
- Interface de controle injetada na página  
- Sistema de auto-paginação  

## Instalação e Uso

O script pode ser usado diretamente no navegador ou via extensão de userscript (como Tampermonkey).

### Para usar manualmente:
  1. Abra o arquivo Script.js
  2. Copie tudo
  3. Crie um favorito e no campo URL cole o script
  4. Abra o elefante letrado e execute o favorito

### Para usar Tampermonkey (Recomendado):
  1. Instale a extensão Tampermonkey no navegador
  2. Crie um novo script
  3. Cole o conteúdo do Script.js
  4. Salve e ative o script
  5. Acesse a plataforma normalmente

# Atenção❗

O script depende de um campo de contexto onde o usuário informa o conteúdo base do livro ou atividade atual. Esse contexto é usado como referência para interpretar perguntas e gerar respostas mais coerentes.

### 🔑 API utilizada

O projeto utiliza a API da [OpenRouter](https://openrouter.ai)

### É necessário:

* Criar uma conta no OpenRouter
* Gerar uma API key em [OpenRouter Key](https://openrouter.ai/workspaces/default/keys)
* Inserir no arquivo Config.js em `OPENROUTER_KEY`
