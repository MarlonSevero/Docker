# 🐳 Docker Images Repo

Este repositório contém **Dockerfiles** e recursos relacionados para a criação de imagens Docker personalizadas, e sendo utilizadas para subir uma pagina simples PHP + Mysql com um Nginx na frente fazendo um load balancer simples.
---

---

## 🛠️ Imagens disponíveis
| Pasta     | Descrição                                | Porta padrão | Base       |
|-----------|------------------------------------------|--------------|------------|
| `web/`    | Imagem com Apache + PHP                  | `80`         | CentOS 7   |
| `mariadb/`| Imagem do mariadb                        | `3306`       | Debian     |
| `nginx/`  | Imagem do nginx			       | `80`	      | Debian	   |
| `jenkins/`| Imagem do Jenkins                        | `50000`      | Debian     |

---

## 📦 Exemplo de como construir as imagens e rodar um container docker.

Você pode construir as imagens no diretorio onde realizou o `git clone`:

```bash
🧱 Primeiro Contruir as imagens
docker compose build

🚀 Segundo rodar o `docker compose up` para inicializar os container
docker compose up -d 

🌐 Terceiro acesso ao container
Após subir a imagem web, acesse via navegador:
http://127.0.0.1:5555




