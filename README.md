# CLI for interacting with Cloudflare in a Docker container

[![IRC Channel](https://img.shields.io/badge/irc-%23giantswarm-blue.svg)](https://kiwiirc.com/client/irc.freenode.net/#giantswarm)

`docker-cloudflare-cli` is a Docker wrapper for [danielpigott/cloudflare-cli](https://github.com/danielpigott/cloudflare-cli).

## Getting docker-cloudflare-cli

Download the latest release: https://github.com/giantswarm/docker-cloudflare-cli/releases/latest

Clone the git repository: https://github.com/giantswarm/docker-cloudflare-cli.git

## Running docker-cloudflare-cli

You can run the `cfcli` command via the Docker container with bind mounting a
`.cfcli.yml` to `/root/.cfcli.yml`:
```
docker run --rm -it \
  -v ~/.cfcli.yml:/root/.cfcli.yml
  giantswarm/docker-cloudflare-cli \
  listdomains
```

## Contact

- Mailing list: [giantswarm](https://groups.google.com/forum/#!forum/giantswarm)
- IRC: #[giantswarm](irc://irc.freenode.org:6667/#giantswarm) on freenode.org
- Bugs: [issues](https://github.com/giantswarm/docker-cloudflare-cli/issues)

## Contributing & Reporting Bugs

See [CONTRIBUTING](CONTRIBUTING.md) for details on submitting patches, the
contribution workflow as well as reporting bugs.

## License

docker-cloudflare-cli is under the Apache 2.0 license. See the [LICENSE](LICENSE) file for details.
