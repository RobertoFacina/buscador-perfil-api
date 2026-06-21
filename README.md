🧑‍💻 Buscador de Perfil de Usuário via API (CLI)

Este projeto é uma aplicação de linha de comando (CLI) desenvolvida em Python que consome a API REST DummyJSON para buscar e exibir informações detalhadas de perfis de usuários.

O objetivo principal deste projeto é demonstrar a capacidade de realizar requisições HTTP, tratar retornos em formato JSON com múltiplos níveis de aninhamento (nested dictionaries) e exibir os dados de forma limpa e estruturada no terminal.

🚀 Funcionalidades

Busca Dinâmica: Capacidade de buscar qualquer usuário passando seu ID na URL da API.

Extração Profunda de Dados: Utilização de encadeamento seguro (.get().get()) para acessar chaves que estão dentro de outros objetos JSON (como endereço e informações da empresa do usuário), evitando que o sistema quebre caso o dado falte na API.

Tratamento de Exceções de Rede: Captura de erros de conexão e falhas de requisição (requests.exceptions.RequestException) para garantir que o usuário receba uma mensagem de erro amigável em vez de um travamento do sistema.

Formatação de Saída: Uso avançado de f-strings para concatenar e exibir os dados de forma profissional e legível.

🛠️ Tecnologias Utilizadas

Python 3.x

Biblioteca requests: Para realizar as chamadas HTTP (GET) para o endpoint da API.

Biblioteca json (Nativa): Para decodificação da resposta.

⚙️ Como executar o projeto

Pré-requisitos

Certifique-se de ter o Python instalado na sua máquina e a biblioteca requests instalada no seu ambiente virtual.

Clone o repositório:

git clone https://github.com/RobertoFacina/buscador-perfil-api.git
cd buscador-perfil-api


Instale a dependência de requisições:

pip install requests


Execute o script:

python buscador_usuario.py


🖥️ Exemplo de Saída no Terminal

Ao rodar o script buscando o ID de usuário 4, o terminal exibirá:

--- Perfil do Usuário 4 ---
Nome: Arthur Frazier
Idade: 50 anos
Email: alittle3@mac.com
Localização: Louisville - KY
Trabalho: IT Manager na Keebler LLC
------------------------------


💡 Habilidades Demonstradas neste Projeto

Consumo de APIs RESTful.

Manipulação defensiva de Dicionários em Python (prevenção do erro KeyError).

Tratamento de exceções e erros de rede.

Boas práticas de modularização com o uso do bloco if __name__ == "__main__":.
