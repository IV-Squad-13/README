📋 Descrição Geral
    O Sistema de Especificações e Catálogo da Construtora Jotanunes é uma aplicação web desenvolvida para gerenciar empreendimentos, materiais, ambientes, itens, usuários e histórico de alterações de forma centralizada. O objetivo é padronizar e digitalizar as informações técnicas das obras, tornando o fluxo entre as equipes de engenharia, arquitetura e administração mais ágil e seguro.
🧠 Principais Funcionalidades
    • Login e autenticação com controle de sessão e perfis de acesso.
    • Gerenciamento de catálogo de ambientes e itens.
    • Cadastro detalhado de empreendimentos, materiais e marcas.
    • Histórico de alterações com controle de versões.
    • Gerenciamento de usuários com permissões específicas.
🧩 Perfis de Acesso
    Tipo de Usuário
    Permissões Principais
    Administrador
    Gerência usuários, catálogo e especificações.
    Gestor
    Cadastra empreendimentos e materiais.
    Redator
    Cria e edita conteúdos técnicos.

⚙️ Guia de Configuração do Ambiente
🐳 Configuração com Docker
      1. Clone o repositório central com submódulos:
         git clone --recurse-submodules https://github.com/iv-squad-13/central.git
      2. Troque para a branch de build: git switch build/image
      3. Verifique as variáveis no docker-compose.yml (Postgres, Mongo e ALLOWED_ORIGINS).
      4. Execute o container:
      docker compose up -d monolito_api client
🧱 Build Local (sem Docker)
      1. Clone o repositório central: git clone --recurse-submodules https://github.com/iv-squad-13/central.git
      2. Entre na pasta /docker e execute: docker compose up
💻 Configuração do Frontend
      Dependências: Node.js e npm instalados, API rodando localmente ou remotamente.
      1. Entre na pasta FrontEnd-JotaNunes e execute: npm install
      2. Execute: npm run dev
☕ Configuração da API
    Dependências: JDK 21, Maven, PostgreSQL e MongoDB (opcionais).
    1. Configure o arquivo .env.properties com as variáveis necessárias.
    2. Execute a aplicação: ./mvnw spring-boot:run
    3. Acesse a documentação: http://localhost:8080/swagger-ui/index.html
🧠 Tecnologias Utilizadas
    Camada
    Tecnologias
    Frontend
    React / Vite / Tailwind / TypeScript
    Backend
    Java Spring Boot
    Banco de Dados
    PostgreSQL / MongoDB
    Ambiente
    Docker / Docker Compose
    Versionamento
    Git e GitHub
    Documentação API
    Swagger UI

📁 Estrutura do Projeto
/central
 ├── /api-monolito        # API principal (Spring Boot)
 ├── /FrontEnd-JotaNunes  # Frontend React
 ├── /docker              # Arquivos Docker Compose e variáveis
 ├── README.md
 └── .env / configs
👨‍💻 Equipe de Desenvolvimento
    • Daniel de Oliveira Mendonça Mota - Front End
    • Fábio Tarcísio Cardoso Moura - Back-End
    • Rafael Gonçalvez Menezes - Back-End
    •  Anthony Yuri Feitosa França - Back-End
🏢 Sobre a Jotanunes Construtora
    A Jotanunes Construtora é referência em qualidade e inovação no setor da construção civil. Este sistema foi desenvolvido para modernizar o gerenciamento de especificações técnicas, garantindo padronização, rastreabilidade e eficiência em todas as etapas do processo construtivo.
📅 Versão Atual
    Versão: 1.0 — Outubro / 2025
📜 Licença
    Projeto de uso interno da Construtora Jotanunes. A reprodução ou redistribuição não autorizada é estritamente proibida.
