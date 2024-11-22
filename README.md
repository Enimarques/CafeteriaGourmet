# Cafeteria Gourmet - Projeto WordPress

Este repositório contém os arquivos necessários para rodar o site **Cafeteria Gourmet**, criado com WordPress. Siga as instruções abaixo para configurar o ambiente e executar o projeto localmente.

---

## **Pré-requisitos**
Antes de começar, certifique-se de que você possui o seguinte instalado no seu computador:
1. **XAMPP** (ou outro servidor local PHP)
   - Baixe e instale a versão mais recente: [XAMPP Download](https://www.apachefriends.org/download.html)
2. **MySQL** (vem incluso no XAMPP).
3. **Git** (para clonar este repositório).
4. Navegador Web (Google Chrome, Firefox, etc.).

---

## **Passo 1: Clonar este repositório**
Abra o terminal ou prompt de comando e execute:

```bash
git clone https://github.com/Enimarques/CafeteriaGourmet.git
Passo 2: Configurar o ambiente
Mover arquivos para o XAMPP:

Copie a pasta do projeto (CafeteriaGourmet) para a pasta htdocs dentro do diretório onde o XAMPP foi instalado.
O caminho deve ser algo como: C:/xampp/htdocs/CafeteriaGourmet.
Configurar o banco de dados:

Inicie o servidor MySQL no painel de controle do XAMPP.
Acesse o phpMyAdmin (geralmente disponível em http://localhost/phpmyadmin).
Crie um banco de dados com o nome cafeteria_gourmet.
Importar o banco de dados:

No phpMyAdmin, selecione o banco de dados criado.
Clique em Importar e selecione o arquivo cafeteriagourmet.sql (disponível neste repositório).
Confirme a importação.
Configurar o WordPress:

Abra o arquivo wp-config.php na pasta do projeto.
Configure as credenciais do banco de dados:
define('DB_NAME', 'cafeteria_gourmet');
define('DB_USER', 'root'); // Usuário do MySQL
define('DB_PASSWORD', ''); // Senha do MySQL
define('DB_HOST', 'localhost'); // Geralmente localhost
Passo 3: Executar o projeto
Inicie os serviços Apache e MySQL no painel de controle do XAMPP.
Acesse o site no navegador em: http://localhost/CafeteriaGourmet.
Estrutura do projeto
wp-content/themes/: Contém o tema personalizado do site.
wp-content/plugins/: Contém plugins utilizados no site.
cafeteriagourmet.sql: Dump do banco de dados.
