# 🐳 Docker Images Repo

Este repositório contém **Dockerfiles** e recursos relacionados para a criação de imagens Docker personalizadas, e sendo utilizadas para subir uma pagina simples PHP + Mysql

---

---

## 🛠️ Imagens disponíveis
| Pasta     | Descrição                                | Porta padrão | Base       |
|-----------|------------------------------------------|--------------|------------|
| `web/`    | Imagem com Apache + PHP                  | `80`         | CentOS 7   |
| `mariadb/`| Imagem do mariadb                        | `3306`       | Debian     |
| `nginx/`  | Imagem do nginx			               | `80`	      | Debian	   |


---

## 📦 Exemplo de como construir as imagens e rodar um container docker.

Você pode construir qualquer imagem com o comando abaixo:

```bash
🧱 Primeiro Contruir as imagens
docker compose build

🚀 Segundo rodar um container
docker compose up -d 

🌐 Terceiro acesso ao container
Após subir a imagem web, acesse via navegador:
http://ip_host:5555




