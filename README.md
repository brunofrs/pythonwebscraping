# Python Web scraping

Objetivo: 

Realizar um Web Scraping na interface WEB do meu roteador para retornar informações do sistema e hosts conectados de forma mais rápida. 

O que precisa ser feito para o código funcionar?

- Copiar o cabeçalho da requisição HTTP e os cookies de acesso para logar na interface sem a necessidade de login e senha. Conforme a imagem abaixo, segue um exemplo de como copiar o cabeçalho de uma requisição junto com os cookies de acesso:

F12(acessar console do desenvolvedor) > Rede > Clique com botão direito na requisição da página, no meu caso era index.html > copiar > Copiar tudo como cURL (bash). 

![image](https://curlconverter.com/images/chrome.webp)


Após copiar o conteúdo, vamos usar o site https://curlconverter.com/python/ para converter a saída do comando cURL para python. Após a conversão, copie o conteúdo e cole no arquivo do código python. 

Observações:

- No caso do meu roteador, as informações do sistema eram passadas através de um link com conteúdo em JSON para o Front-end, que montava a interface WEB de forma mais rápida transformando o conteúdo todo em HTML logo após. Então ao invés de fazer um scraping utilizando as tags HTML onde estavam armazenados os valores, informei diretamente a URL onde o Back-end processava o JSON com todas as informações necessárias para o retorno dos dados ser mais eficiente.

- Caso esse código seja utilizado por terceiros, é necessário modelar ele de acordo com a interface de sua escolha, caso contrário não irá funcionar.
