# Configurando o Projeto

## Subindo o Banco de Dados

1. **Inicie o Docker Compose:**
   Execute o comando abaixo para subir o banco de dados em um contêiner Docker:

   `docker compose up -d`

1. **Acessando o Banco de Dados:**
   Abra um terminal no contêiner MySQL:

   `docker compose exec mysql bash`

1. **Login no MySQL:**
   Efetue o login no MySQL com as credenciais:

   `mysql -uroot -p imersao17`

   Digite a senha quando solicitado, usando "root".

1. **Importando o Esquema do Banco de Dados:**
   No terminal MySQL, assim que estiver disponível, copie todo o conteúdo do arquivo "db.sql":

   Use `Ctrl+A` para selecionar todo o texto e `Ctrl+C` para copiar.
   Cole no terminal do MySQL usando o botão direito do mouse e pressione "Enter".

1. **Verificando as Tabelas Criadas:**
   Após importar o esquema, execute o comando para verificar se as tabelas foram criadas com sucesso:

   `show tables;`

## Executando o Servidor Go

1. **Navegando até o Diretório do Projeto:**
   Abra um novo terminal e navegue até o diretório do projeto

2. **Executando o Servidor Go:**
   Vá até a pasta cmd/catalog e execute o seguinte comando:

   `go run main.go`

   Agora o servidor Go estará em execução.
