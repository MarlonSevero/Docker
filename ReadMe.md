# 🐳 Docker Images Repo

Este repositório contém **Dockerfiles** e recursos relacionados para a criação de imagens Docker personalizadas, utilizadas em diversos projetos (ex: servidores web, monitoramento, gateways, etc).

---

---

## 🛠️ Imagens disponíveis
| Pasta     | Descrição                                | Porta padrão | Base       |
|-----------|------------------------------------------|--------------|------------|
| `web/`    | Imagem com Apache + PHP                  | `80`         | CentOS 7   |
| `mariadb/`| Container do mariadb                     | `3306`       | Debian     |
---

## 📦 Exemplo de como construir as imagens e rodar um container docker.

Você pode construir qualquer imagem com o comando abaixo:

```bash
🧱 Primeiro Contruir a imagem
docker build -t nome-da-imagem ./pasta

🚀 Segundo rodar um container
docker run -d --name meucontainer -p 8080:80 minhaweb

🌐 Terceiro acesso ao container
Após subir a imagem web, acesse via navegador:
http://localhost:8080



