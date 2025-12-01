# TCC - Curso Técnico em Informática para Internet

**Sistema de Gerenciamento de Compra e Venda na Cantina**

Um sistema web desenvolvido como Trabalho de Conclusão de Curso (TCC) para o curso técnico em Informática para Internet. Esta aplicação tem como objetivo Sistema web desenvolvido para otimizar o atendimento da cantina do SENAI/SC em Joinville Sul. A plataforma permite que alunos realizem pedidos e pagamentos antecipadamente pelo celular, eliminando as longas filas físicas, agilizando o processo e melhorando a experiência durante os intervalos.

## Funcionalidades

### Para os Alunos
*   **Cadastro e Acesso:** Crie sua conta e faça login de forma segura.
*   **Cardápio Digital:** Navegue pelo catálogo completo de produtos com preços e disponibilidade.
*   **Pedidos pelo Celular:** Monte seu pedido no carrinho e finalize em poucos cliques.
*   **Acompanhamento em Tempo Real:** Veja o status do seu lanche (ex: "Preparando", "Pronto").
*   **Histórico:** Consulte todos os seus pedidos anteriores.

### Para a Cantina
*   **Painel de Controle:** Interface única para gerenciar pedidos, produtos e estoque.
*   **Controle de Pedidos:** Atualize o status dos pedidos e organize a produção.
*   **Gestão do Cardápio:** Adicione, edite ou desative itens do cardápio facilmente.
*   **Relatórios de Vendas:** Insights sobre os produtos mais vendidos e faturamento.

## Tecnologias Utilizadas

Este projeto foi construído com as seguintes tecnologias:

*   **Backend:** PHP 8.x com o framework **Laravel**
*   **Frontend:** **Bootstrap 5**, JavaScript, HTML5, CSS3
*   **Banco de Dados:** **MySQL**
*   **Ferramentas de Desenvolvimento:** Composer, NPM

## Pré-requisitos

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
*   [Git](https://git-scm.com)
*   [PHP](https://www.php.net/) (versão 8.0 ou superior)
*   [Composer](https://getcomposer.org/)
*   [Node.js](https://nodejs.org/en/) (que inclui o NPM)
*   Um servidor de banco de dados (recomendamos o [MySQL](https://www.mysql.com/) ou [XAMPP](https://www.apachefriends.org/)/[Laragon](https://laragon.org/))

## Instalação e Configuração

Siga estes passos para configurar o projeto localmente:

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/S3rvulo/TCC-Informatica_para_Internet.git
    cd TCC-Informatica_para_Internet/TCC
    ```

2.  **Instale as dependências do PHP (Laravel):**
    ```bash
    composer install
    ```

3.  **Instale as dependências do JavaScript (Bootstrap):**
    ```bash
    npm install
    ```

4.  **Configure o ambiente:**
    *   Copie o arquivo `.env.example` para um novo arquivo chamado `.env`:
        ```bash
        cp .env.example .env
        ```
    *   Gere uma nova chave de aplicação:
        ```bash
        php artisan key:generate
        ```
    *   No arquivo `.env`, configure as variáveis do seu banco de dados (`DB_DATABASE`, `DB_USERNAME`, `DB_PASSWORD`).

5.  **Execute as migrações do banco de dados:**
    ```bash
    php artisan migrate
    ```
    *(Opcional) Para popular o banco com dados de exemplo:*
    ```bash
    php artisan db:seed
    ```

6.  **Compile os assets do frontend:**
    ```bash
    npm run dev
    ```

7.  **Inicie o servidor de desenvolvimento:**
    ```bash
    php artisan serve
    ```

8.  Acesse a aplicação no seu navegador em: `http://localhost:8000`.

## Estrutura do Projeto

TCC/
├── app/ # Lógica da aplicação Laravel (Models, Controllers)
├── bootstrap/
├── config/ # Arquivos de configuração
├── database/ # Migrations, Seeders e Factories
├── public/ # Ponto de entrada público (index.php, assets compilados)
├── resources/
│ ├── js/ # Arquivos JavaScript
│ ├── sass/ # Estilos SASS/SCSS
│ └── views/ # Blade templates (HTML da aplicação)
├── routes/ # Definição das rotas (web.php, api.php)
├── storage/
├── tests/
├── vendor/
├── .env.example # Modelo de variáveis de ambiente
├── artisan # CLI do Laravel
├── composer.json
└── package.json

## Como Contribuir

Contribuições são muito bem-vindas! Este é um projeto acadêmico, mas sugestões são valiosas.

1.  Faça um **Fork** do projeto.
2.  Crie uma **Branch** para sua feature ou correção (`git checkout -b feature/minha-feature`).
3.  **Commit** suas alterações (`git commit -m 'feat: Adiciona nova funcionalidade X'`).
4.  Faça um **Push** para a branch (`git push origin feature/minha-feature`).
5.  Abra um **Pull Request** explicando suas mudanças.

## Licença

Este projeto foi desenvolvido para fins acadêmicos. Consulte o arquivo [LICENSE](LICENSE.md) para mais detalhes.

## Autor

**Seu Nome**
*   GitHub: [@S3rvulo](https://github.com/S3rvulo)
*   LinkedIn: [PEDRO SERVULO PEIXOTO SILVA]([https://linkedin.com/in/seu-perfil](https://www.linkedin.com/in/pedro-servulo-peixoto-silva-482897398/))

## Agradecimentos

*   Agradecimento aos professores e colegas do curso.
*   Às documentações oficiais do [Laravel](https://laravel.com/docs) e [Bootstrap](https://getbootstrap.com/docs/).
*   À comunidade de código aberto.
