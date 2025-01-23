<table align="center">
    <tr>
        <td align="center" width="25%">
            <img src="https://vignette.wikia.nocookie.net/megaman/images/2/22/Cutman.png" alt="MegaMan Bosses API" >
        </td>
        <td align="center" width="75%">
          
# MegaMan Bosses API
          
[![Release workflow](./_docs/assets/icon.png)](https://github.com/Diniciu/MegaApiDotnetCore/actions/workflows/release.yml)
  <br>
        </td>
    </tr>
</table>

<p align="center">
  Este projeto é uma API feita em .NET Core 3.1 que lista dados dos bosses de MegaMan. O objetivo principal é fornecer dados em formato JSON sobre os bosses do jogo.
  <br />
</p>

## Estrutura do JSON

A API fornece dados no seguinte formato:

```json
{
  "Id": 1,
  "Code": "DLN/DRN-003",
  "Name": "Cutman",
  "HP": 150,
  "Picture": "./_docs/assets/carbon.png"
}
```

## Endpoints

| Método | Rota | Descrição |
| --- | --- | --- |
| GET | `/api/v1/robots` | Retorna a lista de todos os bosses. |
| GET | `/api/v1/robots/{id}` | Retorna os dados de um boss específico pelo ID. |
| POST | `/api/v1/robots` | Cria um novo boss. |

## Dependências do Projeto

| Dependência | Descrição |
| --- | --- |
| [Microsoft.EntityFrameworkCore](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/3.1.8) | Provedor de acesso a dados para .NET |
| [Microsoft.EntityFrameworkCore.Design](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/3.1.8) | Ferramentas de design do Entity Framework Core |
| [Microsoft.EntityFrameworkCore.SqlServer](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.8) | Provedor SQL Server para Entity Framework Core |
| [Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json/12.0.2) | Biblioteca para trabalhar com JSON no .NET |

## Estrutura do Projeto

- .vs/
- .vscode/
- bin/
- Controllers/
- Database/
- middlewares/
- Models/
- obj/
- Properties/
- Services/
- appsettings.Development.json
- appsettings.json  
- global.json
- MegamanApi.csproj  
- MegamanApi.sln
- Program.cs
- Startup.cs

## Técnicas Utilizadas

Este projeto utiliza as seguintes técnicas:

- **Programação Orientada a Objetos (POO)**: Para estruturação e organização do código.
- **Injeção de Dependência**: Para gerenciar as dependências e promover um código desacoplado.
- **API RESTful**: Para criação dos endpoints e manipulação dos dados.
- **Entity Framework Core**: Para mapeamento objeto-relacional (ORM) e acesso ao banco de dados.

## Tecnologias Utilizadas

Este projeto utiliza as seguintes tecnologias:

- .NET Core 3.1
- Entity Framework Core
- SQL Server
- Newtonsoft.Json

## Como Executar o Projeto

1. Clone o repositório:

```bash
git clone https://github.com/Diniciu/MegaApiDotnetCore.git
cd megaman-bosses-api
```

2. Restaure as dependências:

```bash
dotnet restore
```

3. Execute o projeto:

```bash
dotnet run
```

## Arquitetura

```🌐
src
├── 📂 Controllers      [Routes for endpoints]
├── 📂 Models           [Database models]
├── 📂 Services         [Business rules]
├── 📂 Middlewares      [Intermediate functions between the HTTP request and the final server response]
├── 📂 Database         [Structures related to the database]
│   ├── 📂 DTOs             [Input Models and View Models (Data Transfer Objects)]
│   ├── 📂 EntityFramework  [Files related to the ORM Entity Framework]
│   │     ├── 📂 Context         [Entity context settings]
│   │     ├── 📂 Migrations      [Migrations for database updates]
│   ├── 📂 Repositories     [Repository pattern]
```

4. Perfil:

⌨ Vinícius Ferreira -
[GitHub](https://github.com/Diniciu)
