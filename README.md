# terraform_aws_ec2_test

Terratest é uma biblioteca Go desenvolvida na Gruntwork, que facilita a escrita de testes automatizados para nosso código de infraestrutura. Ele fornece uma variedade de funções auxiliares e padrões para tarefas comuns de teste de infraestrutura, mas aqui discutiremos sobre como testar o código do Terraform.

# Para executar este aplicativo

- git clone
- cd test <br />
- go mod init "<MODULE_NAME>" <br />
- **MODULE_NAME would be github.com/<YOUR_USERNAME>/<YOUR_REPO_NAME>** <br />
- go mod init github.com/imnitin28/terra-form-test-techhub <br />
- go run

---

go mod init "<MODULE_NAME>" criaria o arquivo go.mod na pasta de teste. <br />

- O arquivo go.mod é a raiz do gerenciamento de dependências no GoLang.
- Todos os módulos que são necessários ou serão utilizados no projeto são mantidos aqui no arquivo go.mod.
- Cria entrada para todos os pacotes que vamos usar/importar em nosso projeto.
- Reduz o esforço para obter cada dependência manualmente.

Ao executar **go test** pela primeira vez, você obteria o arquivo go.sum criado.

- O arquivo go.sum é criado quando **go test** ou **go build** é executado pela primeira vez.
- Instala todos os pacotes com versão específica (mais recente)
- não precisamos editar ou modificar este arquivo.
