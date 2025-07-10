# 🐳 Docker Images Repo

Este repositório contém **Dockerfiles** e recursos relacionados para a criação de imagens Docker personalizadas, utilizadas em diversos projetos (ex: servidores web, monitoramento, gateways, etc).

---

---

## 🛠️ Imagens disponíveis

| Pasta     | Descrição                               | Porta padrão | Base       |
|-----------|------------------------------------------|--------------|------------|
| `web/`    | Imagem com Apache + PHP                  | `80`         | CentOS 7   |
| `zabbix/` | Container do agente/servidor Zabbix      | `10050`      | Debian/Alma|

---

## 📦 Como construir as imagens

Você pode construir qualquer imagem com o comando abaixo:

```bash
docker build -t nome-da-imagem ./pasta

🚀 Como rodar um container
docker run -d --name meucontainer -p 8080:80 minhaweb

🌐 Exemplo de acesso
Após subir a imagem web, acesse via navegador:
http://localhost:8080



