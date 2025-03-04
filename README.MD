# 🌸 API de Robôs Mega Man  
**(MEGA-MAN-ROBOTS)**  

## 🚀 Último Lançamento  
Esta API .NET Core foi projetada para servir dados formatados em JSON sobre os chefes da série Mega Man. É um serviço de backend criado com .NET Core 3.1 e diversas dependências modernas para gerenciamento de dados e tratamento de respostas da API.  

Desenvolvida com o Entity Framework Core e outras tecnologias .NET modernas, esta API tem como objetivo fornecer uma solução robusta para acessar dados dos robôs da série Mega Man.  

---

## 🌟 Pontos de Extremidade da API  

| Método   | Ponto Final               | Descrição                                   |  
|----------|---------------------------|-------------------------------------------|  
| `GET`    | `/api/v1/robôs`           | Retorna uma lista de todos os robôs.       |  
| `GET`    | `/api/v1/robôs/{id}`      | Retorna detalhes de um robô específico por ID. |  
| `POST`   | `/api/v1/robôs`           | Cria uma nova entrada de robô.             |  

---

## 🛠️ Técnicas Utilizadas  
- **Entity Framework Core:** ORM para gerenciamento de dados.  
- **Design de API RESTful:** Garante pontos de comunicação claros e eficazes.  
- **Injeção de Dependência:** Promove acoplamento flexível e capacidade de teste aprimorada.  

---

## 📦 Dependências  

| Pacote                           | Versão   | Link       |  
|----------------------------------|----------|------------|  
| Microsoft.EntityFrameworkCore    | 3.1.8    | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/3.1.8) |  
| Microsoft.EntityFrameworkCore.Design | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/3.1.8) |  
| Microsoft.EntityFrameworkCore.SqlServer | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.8) |  
| Newtonsoft.Json                  | 12.0.2   | [NuGet](https://www.nuget.org/packages/Newtonsoft.Json/12.0.2) |  

---

## 🗂️ Estrutura do Projeto  

```plaintext
src  
├── 📂 Controllers      [Rotas para os endpoints]  
├── 📂 Models           [Modelos do banco de dados]  
├── 📂 Services         [Regras de negócio]  
├── 📂 Middlewares      [Funções intermediárias entre a requisição HTTP e a resposta final do servidor]  
├── 📂 Database         [Estruturas relacionadas ao banco de dados]  
│   ├── 📂 DTOs             [Modelos de entrada e modelos de visualização (Data Transfer Objects)]  
│   ├── 📂 EntityFramework  [Arquivos relacionados ao ORM Entity Framework]  
│   │     ├── 📂 Context         [Configurações do contexto da entidade]  
│   │     ├── 📂 Migrations      [Migrações para atualizações do banco de dados]  
│   ├── 📂 Repositories     [Padrão de repositório]  
