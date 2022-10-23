# Static site example

Simple workflows to view and build static site stuff.

## Getting started

The following tools must be installed to follow along.

- Pandoc
- Docker Cli
- Docker Compose

Clone this repo.

```shell
git clone https://github.com/JulioPDX/static-hosting-example.git
cd static-hosting-example
```

## Install Python requirements

```shell
python3 -m venv venv
source venv/bin/activate
pip install -r avd-project/req.txt
```

## View MkDocs site

```shell
mkdocs serve
```

## Build MkDocs site

```shell
mkdocs build
```

## Run site on container

```shell
docker-compose up --build
```

## References

- [Pandoc](https://pandoc.org/)
- [Pandoc CSS](https://gist.github.com/killercup/5917178)
- [MkDocs](https://www.mkdocs.org/)
- [MkDocs Material Theme](https://squidfunk.github.io/mkdocs-material/)
- [Simple MkDocs navigation plugin](https://github.com/mysiki/mkdocs_include_dir_to_nav)
- [Docker and Docker Compose install](https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/How-to-install-Docker-and-docker-compose-on-Ubuntu)
- [Very light container to display static site](https://lipanski.com/posts/smallest-docker-image-static-website)
- [GitHub for container image](https://github.com/lipanski/docker-static-website)
- [AVD and Docs running on Docker or Kubernetes by Thomas Grimonet](https://github.com/titom73/demo-avd-compose-k8s)
