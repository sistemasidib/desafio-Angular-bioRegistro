# Desafio Angular - Desenvolvedor Júnior/Pleno

Este repositório contém um desafio técnico para a vaga de Desenvolvedor Angular Júnior/Pleno. O objetivo deste desafio é avaliar as habilidades em desenvolvimento frontend, boas práticas de código, e capacidade de realizar o deploy de uma aplicação web.

## 🏆 Objetivo do Desafio

Desenvolver uma aplicação web em Angular que permita:
- Criar, atualizar, listar e excluir registros de uma entidade (ex: Tarefas, Produtos, Usuários).
- Implementar autenticação básica (JWT).
- Realizar consumo de uma API REST.

### Requisitos Técnicos (Obrigatórios):
- **Utilizar Angular 18 (obrigatório)**, com as novas features como **Angular Signals** e o padrão **Standalone Components**.
- Utilizar TypeScript e seguir boas práticas de desenvolvimento.
- Implementar tratamento de erros e validações.

### Extras (Diferenciais):
- Implementar lazy loading.
- Utilizar bibliotecas de componentes (ex: Angular Material, PrimeNG).
- Implementar paginação e filtros.

## 📦 Como Executar o Projeto Localmente

Para rodar a aplicação em ambiente local:

1. **Clone o Repositório:**
```bash
git clone https://github.com/sistemasidib/desafio-Angular-bioRegistro.git
```
2. **Instalar Dependências:**
```bash
npm install
```
3. **Executar a Aplicação:**
```bash
ng serve
```
4. **Acessar a Aplicação:**
   - A aplicação estará disponível em `http://localhost:4200`.

## 🚀 Deploy usando Docker e NGINX

### Configuração Docker

1. **Construção da Imagem:**
```bash
docker build -t minha-app-angular .
```
2. **Executar o Container:**
```bash
docker run -d -p 80:80 --name minha-app-angular minha-app-angular
```

### Configuração NGINX (Proxy Reverso)

```nginx
server {
    listen 80;
    server_name app.meudominio.com;

    location / {
        root /usr/share/nginx/html;
        index index.html;
        try_files $uri /index.html;
    }
}
```

## ✅ Critérios de Avaliação
- Utilização obrigatória do **Angular 18** com **Signals** e **Standalone Components**.
- Qualidade do código (organização, boas práticas, padrões de projeto).
- Clareza na documentação.
- Implementação de boas práticas de segurança.
- Capacidade de configurar o ambiente de deploy (Docker e NGINX).

Boa sorte e sucesso no desafio!

