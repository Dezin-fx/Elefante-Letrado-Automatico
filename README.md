# Elefante-Letrado-Automatico

![Status](https://img.shields.io/badge/status-active-brightgreen)
![Platform](https://img.shields.io/badge/platform-browser-blue)
![Type](https://img.shields.io/badge/type-userscript-yellow)

Este script automatiza leitura e questões dentro da plataforma Elefante Letrado. 
Ele é executado no navegador e manipula a interface para reduzir ações manuais durante o uso da plataforma.

## As principais funções são:

- Avançar automaticamente entre páginas ou etapas da atividade quando a página atual já foi processada ou não requer interação manual.
- Identificar momentos em que há perguntas e tentar responder automaticamente com base em um contexto fornecido pelo usuário.
- Utilizar um campo de contexto do livro (ou conteúdo atual) para orientar as respostas geradas, permitindo que o script tente manter coerência com o material exibido.
- Interagir com elementos da interface como botões de continuar, avançar ou confirmar, simulando ações do usuário.

## Instalação e Uso

O script pode ser usado diretamente no navegador ou via extensão de userscript (como Tampermonkey).

### Para usar manualmente:
  1. Abra o arquivo Script.js
  2. Copie tudo
  3. Crie um favorito e no campo URL cole o script
  4. Abra o elefante letrado e execute o favorito

### Para usar Tampermonkey(Recomendado):
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
* Inserir no arquivo Config.js
