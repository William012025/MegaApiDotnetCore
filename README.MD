<p align="center">
  <img src="./_docs/assets/icon.png" alt="Logo do Projeto" width="15%">
</p>

<h1 align="center" style="font-size: 42px;"><b>MegaMan API</b></h1>


          
[![.NET Core](https://img.shields.io/badge/.NET%20Core-3.1-blue)](https://dotnet.microsoft.com/en-us/)
[![Entity Framework](https://img.shields.io/badge/Entity%20Framework-3.1.8-green)](https://docs.microsoft.com/en-us/ef/)
[![Newtonsoft.Json](https://img.shields.io/badge/Newtonsoft.Json-12.0.2-orange)](https://www.newtonsoft.com/json)
        </td>
    </tr>
</table>

## Sobre o projeto

A **Megaman API** é um backend desenvolvido em **.NET Core 3.1** para fornecer informações sobre os *bosses* da franquia **Megaman**.

A API retorna dados em JSON no seguinte formato:

```json
{
  "Id": 1,
  "Code": "DLN/DRN-003",
  "Name": "Cutman",
  "HP": 150,
  "Picture": "https://vignette.wikia.nocookie.net/megaman/images/2/22/Cutman.png"
}
```

## Estrutura do projeto

```
📁 .vs/
📁 .vscode/
📁 bin/
📁 Controllers/
📁 Database/
📁 middlewares/
📁 Models/
📁 obj/
📁 Properties/
📁 Services/
📄 appsettings.Development.json
📄 appsettings.json
📄 global.json
📄 MegamanApi.csproj
📄 MegamanApi.sln
📄 Program.cs
📄 Startup.cs
```

## Endpoints

| Método | Rota                 | Descrição                         |
|--------|----------------------|---------------------------------|
| GET    | /api/v1/robots       | Retorna todos os robôs        |
| GET    | /api/v1/robots/{id}  | Retorna um robô pelo ID       |
| POST   | /api/v1/robots       | Envia um novo robô            |

## Tecnologias e Técnicas Utilizadas

- **.NET Core 3.1** - Framework principal do projeto ([.NET Core](https://dotnet.microsoft.com/en-us/))
- **Entity Framework Core 3.1.8** - ORM para gerenciar o banco de dados ([Entity Framework](https://docs.microsoft.com/en-us/ef/))
- **ASP.NET Core Web API** - Para construir os endpoints ([ASP.NET Core](https://dotnet.microsoft.com/en-us/apps/aspnet))
- **Newtonsoft.Json 12.0.2** - Biblioteca para manipulação de JSON ([Newtonsoft.Json](https://www.newtonsoft.com/json))

## Dependências

| Pacote | Versão | Link |
|--------|--------|------|
| Microsoft.EntityFrameworkCore | 3.1.8 | [Entity Framework](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/3.1.8) |
| Microsoft.EntityFrameworkCore.Design | 3.1.8 | [EF Core Design](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/3.1.8) |
| Microsoft.EntityFrameworkCore.SqlServer | 3.1.8 | [EF Core SQL Server](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.8) |
| Newtonsoft.Json | 12.0.2 | [Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json/12.0.2) |

## Como Rodar o Projeto

1. Clone o repositório:
   ```sh
   git clone https://github.com/William012025/MegaApiDotnetCore
   ```
2. Navegue até o diretório do projeto:
   ```sh
   cd megaman-api
   ```
3. Restaure as dependências:
   ```sh
   dotnet restore
   ```
4. Inicie o servidor:
   ```sh
   dotnet run
   ```

Agora, a API estará disponível em `https://github.com/William012025/MegaApiDotnetCore`.

## Licença

Este projeto está licenciado sob os termos da licença [MIT](LICENSE).





