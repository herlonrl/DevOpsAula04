# DevOpsAula04 - Desafio Imagem Docker 🚀

Olá, Avanters! Preparados para mais um desafio? 🚀🚀🚀

O desafio deste módulo consiste na **criação de imagens Docker**, publicação no **Docker Hub** e execução das imagens usando o **Docker Compose**.

---

## 🧩 Descrição do Projeto

Temos uma aplicação chamada **"Gerador de Saudações"**, composta por:

- Uma **página principal HTML**.
- Um **microsserviço de saudações aleatórias**.
- Um **microsserviço de pessoas aleatórias**.

A missão é:

1. Criar um `Dockerfile` para **cada uma** das 3 aplicações.
2. Fazer o **build** das imagens.
3. Publicar as imagens no **Docker Hub**.
4. Subir tudo com **Docker Compose**.

---

## 📦 Repositórios e Instruções

### 🔹 Site Gerador de Saudações

- **Código**: [site-gerador-saudacoes](https://gitlab.com/avanti-dvp/site-gerador-saudacoes)
- **Instruções Docker**: [docker.md](https://gitlab.com/avanti-dvp/site-gerador-saudacoes/-/blob/main/docs/docker.md?ref_type=heads)

---

### 🔹 Microsserviço Pessoas Aleatórias

- **Código**: [ms-pessoas-aleatorias](https://gitlab.com/avanti-dvp/ms-pessoas-aleatorias)
- **Instruções Docker**: [docker.md](https://gitlab.com/avanti-dvp/ms-pessoas-aleatorias/-/blob/main/docs/docker.md?ref_type=heads)

---

### 🔹 Microsserviço Saudações Aleatórias

- **Código**: [ms-saudacoes-aleatorias](https://gitlab.com/avanti-dvp/ms-saudacoes-aleatorias)
- **Instruções Docker**: [docker.md](https://gitlab.com/avanti-dvp/ms-saudacoes-aleatorias/-/blob/main/docs/docker.md?ref_type=heads)

---

## ⚙️ Subindo com Docker Compose

Após publicar suas imagens no Docker Hub:

1. Use o `docker-compose.yaml` de exemplo (fornecido nos materiais complementares).
2. Salve o arquivo no seu diretório de trabalho.
3. Execute:

```bash
sudo docker compose up -d
````

⚠️ Lembre-se de rodar este comando na **raiz do diretório** onde está o `docker-compose.yaml`.

---

## 🧹 Limpando as imagens locais

Para garantir que o Docker Compose use as imagens do Docker Hub:

1. Remova as imagens locais com:

```bash
sudo docker rmi <nome_ou_id_da_imagem>
```

2. Se houver contêineres usando essas imagens, pare e remova-os.

3. Ou, se preferir, rode:

```bash
sudo docker system prune -a --volumes
```

> ⚠️ **Atenção**: Este comando é **altamente destrutivo**! Removerá **todos os contêineres, imagens, volumes, etc.** Tire as crianças da sala! 😄

---

## ✅ Entrega

Envie os seguintes itens como evidência:

* O código dos **3 Dockerfiles**.
* O código do **docker-compose.yaml**.
* Uma **captura de tela da página funcionando**.

Boa sorte! 🚀💻
