🚀 Projeto WireMock API
Este repositório contém simuladores de API (Mocks) utilizando o WireMock. O objetivo é mimetizar o comportamento de uma API de carros para testes de integração e desenvolvimento front-end/mobile.

📁 Estrutura do Projeto
mappings/: Contém as definições de requisição e resposta (JSON).

__files/: Contém arquivos de corpo de resposta estáticos.

wiremock-standalone-3.13.2.jar: Executável do servidor WireMock.

🛠️ Pré-requisitos
Para rodar este projeto, você precisa ter o Java (JRE ou JDK) instalado na sua máquina (versão 11 ou superior recomendada).

🏃 Como Rodar o Mock
Abra o terminal na pasta raiz do projeto.

Execute o seguinte comando:

Bash
java -jar wiremock-standalone-3.13.2.jar --port 8080 --verbose
O servidor estará rodando em: http://localhost:8080

🔌 Endpoints MapeadosMétodoEndpointDescriçãoGET/api/carsLista todos os carrosPOST/api/carsRegistra um novo carro (Valida brand, model e year)GET/api/cars/500Simula um erro interno do servidor (500)


Um bom README é essencial para que qualquer pessoa (ou você mesma no futuro) entenda como rodar esses mocks rapidamente. Como você está usando o WireMock standalone, o foco deve ser no comando de execução.

Aqui está um modelo profissional e direto para o seu projeto:

🚀 Projeto WireMock API
Este repositório contém simuladores de API (Mocks) utilizando o WireMock. O objetivo é mimetizar o comportamento de uma API de carros para testes de integração e desenvolvimento front-end/mobile.

📁 Estrutura do Projeto
mappings/: Contém as definições de requisição e resposta (JSON).

__files/: Contém arquivos de corpo de resposta estáticos.

wiremock-standalone-3.13.2.jar: Executável do servidor WireMock.

🛠️ Pré-requisitos
Para rodar este projeto, você precisa ter o Java (JRE ou JDK) instalado na sua máquina (versão 11 ou superior recomendada).

🏃 Como Rodar o Mock
Abra o terminal na pasta raiz do projeto.

Execute o seguinte comando:

Bash
java -jar wiremock-standalone-3.13.2.jar --port 8080 --verbose
O servidor estará rodando em: http://localhost:8080

🔌 Endpoints Mapeados
Método	Endpoint	Descrição
GET	/api/cars	Lista todos os carros
POST	/api/cars	Registra um novo carro (Valida brand, model e year)
GET	/api/cars/500	Simula um erro interno do servidor (500)
🧪 Exemplo de Requisição (POST)
URL: http://localhost:8080/api/cars

Body:

JSON
{
  "brand": "Volkswagen",
  "model": "gol",
  "year": 2023
}
Como adicionar isso ao seu GitHub:
No VS Code, crie um novo arquivo chamado README.md (letras maiúsculas e extensão .md).

Cole o conteúdo acima dentro dele.

Salve o arquivo.

No terminal, envie a atualização para o GitHub:

Bash
git add README.md
git commit -m "docs: adicionando README com instruções de execução"
git push
