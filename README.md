# Clique e Aprenda: Sua IA Educacional a um Toque!

Este projeto utiliza a API do Google Gemini para extrair texto de arquivos PDF, gerar resumos e tópicos principais, e criar um chatbot interativo que faz perguntas sobre o conteúdo do PDF e avalia as respostas do usuário.

## Funcionalidades

*   **Extração de Texto:** Lê e extrai o conteúdo de arquivos PDF.
*   **Resumo Automático:** Gera um resumo conciso do conteúdo do PDF usando a API Gemini.
*   **Identificação de Tópicos:** Lista os principais tópicos e sub-tópicos do PDF.
*   **Chatbot Interativo:**
    *   Gera perguntas sobre o conteúdo do PDF.
    *   Permite ao usuário responder às perguntas.
    *   Avalia as respostas do usuário com base no texto original usando a API Gemini.

## Pré-requisitos

*   Uma conta Google.
*   Acesso à API do Google Gemini. Você precisará gerar uma chave de API.
*   Google Colab ou ambiente Python com Jupyter Notebooks instalado.
*   As bibliotecas `genai` e `PyMuPDF` instaladas.

## Configuração

1.  **Obtenha uma Chave de API do Google Gemini:** Siga as instruções na documentação do Google AI para obter sua chave de API.
2.  **Clone o Repositório:** Clone este repositório para o seu ambiente local.
3.  **Abra no Google Colab:** Abra o arquivo `.ipynb` no Google Colab.
4.  **Configure a Chave de API:**
    *   No Google Colab, vá em "Secrets" (ícone de chave no painel lateral).
    *   Clique em "+ New secret".
    *   Para "Name", digite `GOOGLE_API_KEY`.
    *   Para "Value", cole a sua chave de API do Google Gemini.
    *   Certifique-se de que a opção "Notebook access" esteja ativada.
5.  **Monte o Google Drive:** O notebook inclui código para montar o Google Drive. Isso é necessário para acessar o arquivo PDF.
6.  **Atualize o Caminho do PDF:** No código, localize a linha `caminho_do_pdf = "/content/drive/My Drive/aprendizado.pdf"` e atualize-a com o caminho real para o seu arquivo PDF no Google Drive, ou coloque o PDF na sua pasta raiz do My Drive e renomei-o para aprendizado.pdf mantendo este mesmo caminho.
,
## Como Executar

1.  Siga os passos de configuração acima.
2.  Execute cada célula do notebook em sequência.
3.  O notebook irá:
    *   Montar o Google Drive.
    *   Instalar as bibliotecas necessárias.
    *   Configurar a chave de API.
    *   Extrair o texto do PDF especificado.
    *   Gerar e imprimir o resumo e os tópicos do PDF.
    *   Iniciar o chatbot interativo.
4.  No chatbot, responda às perguntas geradas com base no conteúdo do PDF. Digite 'fim' para encerrar o chat.

## Bibliotecas Utilizadas

*   `google.colab`: Para integração com o Google Colab (montar Drive, Secrets).
*   `genai`: Para interagir com a API do Google Gemini.
*   `PyMuPDF` (importado como `fitz`): Para extração de texto de arquivos PDF.

## Estrutura do Código

O código está organizado em células no notebook Jupyter/Colab:

1.  Importação de bibliotecas.
2.  Montagem do Google Drive.
3.  Instalação das bibliotecas.
4.  Configuração da chave de API do Gemini.
5.  Definição do modelo Gemini a ser usado.
6.  Definição do caminho para o arquivo PDF.
7.  Função para extrair texto do PDF.
8.  Execução da extração de texto e verificação de sucesso.
9.  Geração e impressão do resumo e tópicos usando Gemini.
10. Implementação do chatbot: geração de perguntas e loop de interação com avaliação das respostas.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.

## Licença

Este projeto está licenciado sob a Licença Pública Geral GNU v3.0 .
