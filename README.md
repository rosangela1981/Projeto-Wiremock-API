🚀 Projeto WireMock APIEste repositório contém simuladores de API (Mocks) utilizando o WireMock. O objetivo é mimetizar o comportamento de uma API de carros para testes de integração e desenvolvimento front-end/mobile.📁 Estrutura do Projetomappings/: Contém as definições de requisição e resposta (JSON).__files/: Contém arquivos de corpo de resposta estáticos.wiremock-standalone-3.13.2.jar: Executável do servidor WireMock.🛠️ Pré-requisitosPara rodar este projeto, você precisa ter o Java (JRE ou JDK) instalado na sua máquina (versão 11 ou superior recomendada).🏃 Como Rodar o MockAbra o terminal na pasta raiz do projeto.Execute o seguinte comando:Bashjava -jar wiremock-standalone-3.13.2.jar --port 8080 --verbose
O servidor estará rodando em: http://localhost:8080🔌 Endpoints MapeadosMétodoEndpointDescriçãoGET/api/carsLista todos os carrosPOST/api/carsRegistra um novo carro (Valida brand, model e year)GET/api/cars/500Simula um erro interno do servidor (500)🧪 Exemplo de Requisição (POST)URL: http://localhost:8080/api/carsBody:JSON{
  "brand": "Volkswagen",
  "model": "gol",
  "year": 2023
}
Como adicionar isso ao seu GitHub:No VS Code, crie um novo arquivo chamado README.md (letras maiúsculas e extensão .md).Cole o conteúdo acima dentro dele.Salve o arquivo.No terminal, envie a atualização para o GitHub:Bashgit add README.md
git commit -m "docs: adicionando README com instruções de execução"
git push
