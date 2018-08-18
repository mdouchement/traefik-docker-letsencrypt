# Traefik + Docker + Let's Encrypt

The purpose of this repository is to show an example about how to configure all these services together.

Features:
- Auto TLS with Let's Encrypt and Traefik
- Traefik will automatically expose new container instances using the configured `labels` on the container.

## Usage

In this repository, the configuration lets assume that your domain is `example.com`

1. Clone this repository

  ```sh
  git clone https://github.com/mdouchement/traefik-docker-letsencrypt.git /opt
  ```

2. Create the Docker's network

  ```sh
  docker network create traefik
  ```

3. Goto `traefik/` and follow the readme
4. Got to `shiori/` for an application example

## Licence

MIT. See the [LICENSE](https://github.com/mdouchement/traefik-docker-letsencrypt/blob/master/LICENSE) for more details.

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Launch linter (`gometalinter --config=gometalinter.json ./...`)
4. Commit your changes (`git commit -am 'Add some feature'`)
5. Push to the branch (`git push origin my-new-feature`)
6. Create new Pull Request
