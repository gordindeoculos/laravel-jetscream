# 🚀 Projeto Laravel 12 com Jetstream + Livewire (Ambiente Laragon)

Este projeto foi criado como base para estudos e desenvolvimento com **Laravel 12**, utilizando **Jetstream** com **Livewire** e tradução para **pt_BR**.  
O ambiente de desenvolvimento foi configurado com **Laragon**, e o envio de e-mails locais é feito através do **MailPit**.

---

## 🧩 Tecnologias Utilizadas

- **Laravel 12**
- **PHP 8.2+**
- **Jetstream**
- **Livewire**
- **Tailwind CSS**
- **Vite**
- **MailPit** (para testes de e-mail)
- **Laragon** (ambiente local)

---

## ⚙️ Requisitos do Ambiente

Antes de iniciar, verifique se você possui:

- [Laragon (Full)](https://laragon.org/download/)

---

## 🏗️ Instalação do Projeto

### 1. Clonar o repositório

```bash
git clone https://github.com/gordindeoculos/laravel-jetscream
cd laravel-jetscream
````

### 2. Instalar dependências PHP

```bash
composer install
```

### 3. Instalar dependências JavaScript

```bash
npm install
```

### 4. Criar o arquivo `.env`

Copie o arquivo de exemplo:

```bash
cp .env.example .env
```

Gere a chave da aplicação:

```bash
php artisan key:generate
```

### 5. Configurar o banco de dados

No arquivo `.env`, defina as credenciais do banco de dados local (Laragon):

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=
```

Crie o banco manualmente no **phpMyAdmin** (ou via terminal) e rode as migrações:

```bash
php artisan migrate
```

---

## 🌍 Tradução para Português (pt_BR)

O projeto utiliza o pacote **laravel-lang** para traduzir todas as mensagens padrão.

Instale o pacote:

```bash
composer require laravel-lang/common --dev
```

Adicione o idioma `pt_BR`:

```bash
php artisan lang:add pt_BR
```

Defina o idioma no arquivo `config/app.php`:

```php
'locale' => 'pt_BR',
```

---

## ✉️ Configuração do MailPit (Laragon)

O **MailPit** é utilizado para capturar e-mails de teste localmente.
No Laragon, ative:
**Menu → Mail → MailPit**

Atualize o arquivo `.env` com as configurações abaixo:

```env
MAIL_MAILER=smtp
MAIL_HOST=127.0.0.1
MAIL_PORT=1025
MAIL_USERNAME=null
MAIL_PASSWORD=null
MAIL_ENCRYPTION=null
MAIL_FROM_ADDRESS="teste@local.dev"
MAIL_FROM_NAME="${APP_NAME}"
```

A interface do MailPit estará disponível em:
👉 [http://127.0.0.1:8025](http://127.0.0.1:8025)

---

## 🧠 Recursos Inclusos

✅ Autenticação com Login e Registro
✅ Recuperação de Senha
✅ Gerenciamento de Perfil de Usuário
✅ Tradução completa para pt_BR
✅ Layout padrão com Tailwind CSS
✅ Integração com MailPit para testes de e-mail
✅ Pronto para customização e expansão

---

## 🚀 Executar o Projeto

Inicie o servidor Laravel:

```bash
php artisan serve
```

E o Vite (para assets CSS/JS):

```bash
npm run build
```

Acesse o projeto em:
👉 [http://127.0.0.1:8000](http://127.0.0.1:8000)

---

## 📄 Licença

Este projeto está licenciado sob a **MIT License**.
Sinta-se livre para usar, modificar e distribuir.

---

## 👨‍💻 Autor

**Renato Teixeira Gomes**
Canal: [Gordin de Óculos - Informática e Tecnologia](https://www.youtube.com/@gordindeoculos)
📧 E-mail: [gordindeoculos.dev@gmail.com](mailto:gordindeoculos.dev@gmail.com)

