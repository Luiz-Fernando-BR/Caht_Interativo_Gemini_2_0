# Chat Interativo com Modelo Generativo Gemini

Este projeto implementa um **chat interativo** utilizando o modelo generativo **Gemini 2.0** da Google. Ele permite explorar as capacidades da inteligência artificial generativa em um ambiente dinâmico e amigável, ideal para prototipagem, testes ou aprendizado.

## Funcionalidades

- **Conversa em tempo real**: Permite enviar mensagens para o modelo e receber respostas geradas pela IA de forma imediata.
- **Interface simples**: Interaja diretamente pelo terminal, sem necessidade de configurações avançadas.
- **Controle de encerramento**: Saia facilmente da sessão de chat digitando palavras-chave como `sair`, `exit` ou `quit`.
- **Configurações personalizadas**: Utilize parâmetros ajustáveis, como temperatura, limite de tokens e métodos de amostragem, para controlar o comportamento do modelo.

## Requisitos

- **Python 3.8 ou superior**
- Chave de API válida do Google Generative AI (Gemini 2.0)
- Acesso à internet para comunicação com a API da Google

## Bibliotecas Utilizadas

As bibliotecas necessárias para executar o projeto são:
- **`google.generativeai`**: Biblioteca oficial para integração com os modelos generativos da Google.
- **`os`**: Gerenciamento de variáveis de ambiente (opcional, dependendo da implementação).

## Configuração e Execução

1. Certifique-se de ter uma chave de API válida do **Google Generative AI**:
   - Acesse [Google AI Studio](https://aistudio.google.com/app/apikey) para criar uma chave.
   - Salve a chave em uma variável de ambiente ou insira diretamente no código, conforme necessário.

2. Instale a biblioteca necessária:
   ```bash
   pip install google-generativeai
   ```

3. Clone este repositório e navegue até o diretório do projeto:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   cd seu-repositorio
   ```

4. Execute o código:
   ```bash
   python chat_interativo.py
   ```

5. Interaja com o chat e encerre a sessão digitando `sair`, `exit` ou `quit`.

## Exemplo de Uso

```bash
Você: Olá, IA!
Modelo: Olá! Como posso ajudá-lo hoje?

Você: Qual a previsão do tempo para amanhã?
Modelo: No momento, não tenho acesso a dados de previsão do tempo, mas posso ajudá-lo com outras informações.

Você: sair
Encerrando o chat.
```

## Personalização

- Modifique os parâmetros no dicionário `generation_config` para ajustar o comportamento do modelo:
  - `temperature`: Controle a aleatoriedade das respostas.
  - `top_p` e `top_k`: Ajuste os métodos de amostragem.
  - `max_output_tokens`: Defina o limite de tokens na resposta.
