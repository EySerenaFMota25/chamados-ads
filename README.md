# chamados-ads  
## API de Chamado 
Estudante: Eyshila Serena Ferreira Mota  
## Objetivo:  
Desenvolver uma API Rest em Python da disciplina  "Programação para Web" do curso de Análise e Desenvolvimento de Sistemas (ADS) da Universidade Federal do Cariri (UFCA). Utilizei o framework Flask e o gerencioador de pacotes e ambiente "uv", disponibilizando uma rota inicial para verificação de funcionamento do serviço.  
## Como instalar as dependências?
Certificar-se de ter o `uv` instalado.  
Caso não tenha, você deve instalar com o `pip install uv`.  
Na raiz do projeto, execute o comando a seguir para criar o ambiente virtual e instalar as dependências nas versões exatas registradas no arquivo `uv.lock`:  
```bash  
uv sync --locked  
```  
## Como executar a app?  
Iniciar o servidor Flask localmente ou no GitHub Codespaces, execute:  
```bash  
uv run flask --app app run --host=0.0.0.0 --port=5000  
```  
## Como acessar a rota inicial? Qual a resposta espera?  
Com a aplicação em execução, faça uma requisição `GET` para a rota raiz ('http://localhost:5000/') pelo navegador ou pelo terminal:  
```bash  
curl -i http://localhost:5000/  
```  
**Resposta esperada**  
-> Status HTTP: `200 OK`  
-> Cabeçalho: `Content-Type: application/json`  
-> Corpo (JSON):  
```json  
{  
"mensagem": "API de chamados em funcionamento"  
}  
```
