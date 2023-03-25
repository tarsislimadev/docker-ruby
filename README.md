# Docker Ruby

[![github/actions/workflow/status](https://img.shields.io/github/actions/workflow/status/brtmvdl/docker-ruby/docker-push.yml)](https://img.shields.io/github/actions/workflow/status/brtmvdl/docker-ruby/docker-push.yml) [![github/license](https://img.shields.io/github/license/brtmvdl/docker-ruby)](https://img.shields.io/github/license/brtmvdl/docker-ruby) [![github/stars](https://img.shields.io/github/stars/brtmvdl/docker-ruby?style=social)](https://img.shields.io/github/stars/brtmvdl/antify?style=social)

Para compilaçao e entrega de projetos escritos em Ruby

Veja mais em [hub.docker.com/r/tmvdl/ruby](https://hub.docker.com/r/tmvdl/ruby)

## Como usar

Instalar o [Docker](https://docs.docker.com/engine/install/).

### Em ambiente de desenvolvimento

Criar um arquivo `docker-compose.yaml` na raiz do projeto com a imagem [tmvdl/ruby](https://hub.docker.com/r/tmvdl/ruby).

```yaml
version: '3'

services:
  app:
    image: tmvdl/ruby
    volumes:
      - .:/app
```

Subir o container para a construção do build

```bash
docker-compose up --build
```

### Em ambiente de produção

Executar como container do Docker

```sh
docker run tmvdl/ruby
```

## License

[MIT](./LICENSE) 
