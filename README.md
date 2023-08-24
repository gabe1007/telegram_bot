# Crie um Chatbot💬 no Telegram usando ChatGPT, Flask, and EC2

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-360/)

## Resumo

Este projeto demonstra como criar um chatbot do Telegram usando ChatGPT, Flask e EC2. As seguintes tecnologias e serviços são usados:

- Ngrok e Flask como servidor.
- Token do BOT do Telegram obtido de "BotFather".
- API do ChatGPT para gerar respostas.
- Aplicativo Flask como uma API para o modelo de Requisição/Resposta.
- AWS EC2 para implantação (funcionando 24/7).

## Passos

1. Crie contas gratuitas em OpenAI, AWS e Ngrok.
2. Crie um aplicativo Flask.
3. Crie uma instância EC2 na AWS.
4. Faça o clone deste repositório na instância EC2.
5. Crie um bot do Telegram usando "BotFather" e obtenha o Token da API.
6. Use o TELEGRAM_BOT_TOKEN e OPENAI_API_KEY em seu código (evite usar valores estáticos, use variáveis globais).
7. Execute o script na instância EC2.
8. Abra um segundo terminal e use o Ngrok para criar um túnel na porta 5000.
9. Configure um webhook para verificação do Telegram.

## Uso

Para utilizar este projeto:

1. Clone o repositório.
2. Abra um terminal no diretório de trabalho.
3. Execute o seguinte comando para instalar as dependências necessárias:

    ```
    pip install -r requirements.txt
    ```

4. `telegram_bot.py` é a API Flask que lida com a requisição/resposta do chatbot.
5. Execute o script com o seguinte comando:

    ```
    python3 telegram_bot.py
    ```

6. Para configurar o webhook, use o seguinte formato:

    ```
    https://api.telegram.org/bot<Your Bot Token>/setWebhook?url=<URL of App>
    ```


Sinta-se à vontade para me seguir e dar uma estrela⭐ neste repositório!
