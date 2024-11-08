# Projeto de Tradução de Documentos com Azure Translator

Este projeto é um tradutor de documentos `.docx` que usa a API do Azure Cognitive Services para realizar traduções automáticas de textos em inglês para outros idiomas. O projeto é ideal para traduzir documentos de forma rápida, aproveitando as capacidades do Azure Translator para processar e devolver o texto em diferentes idiomas.

## Pré-requisitos

1. **Conta no Azure** com acesso ao **Azure Cognitive Services** (Translator API).
2. **Chave de assinatura e endpoint** do Azure Translator.
3. **Google Colab** (ou ambiente local com Python 3).

## Instalação

1. Clone este repositório ou copie o código para seu ambiente local ou Google Colab.
2. Instale as bibliotecas necessárias:
    ```python
    !pip install requests python-docx
    ```

## Configuração

Insira sua chave de assinatura e o endpoint do Azure Translator no código. Essas variáveis estão definidas no trecho:

python</br>
subscription_key = "SUA_CHAVE_DE_ASSINATURA"</br>
endpoint = 'SEU_ENDPOINT'</br>
location = "SUA_LOCALIDADE"  # Exemplo: "eastus"</br>


## Uso

Carregue o documento .docx que deseja traduzir para o seu ambiente.</br>
Execute o código no Colab ou ambiente Python.</br>
O código salvará a tradução como um novo arquivo .docx, adicionando o sufixo de idioma ao nome do arquivo original.</br>

## Exemplo de Execução

input_file = "/caminho/para/seu/arquivo.docx"</br>
output_file = translate_document(input_file)</br>
print(f"Arquivo traduzido salvo como: {output_file}")</br>

## Funções Principais</br>
translator_text(text, language_destination): Função que usa a API do Azure Translator para traduzir um trecho de texto.</br>
</br>
translate_document(path): Função que carrega um documento .docx, traduz cada parágrafo e salva o texto traduzido em um novo documento.</br>
</br>
### Contribuição</br>

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests para melhorar o projeto.</br>
</br>
### Licença</br>
</br>
Este projeto é apenas para fins educacionais e é distribuído sem garantia. Consulte os termos de uso da API do Azure Cognitive Services para mais detalhes sobre restrições.
