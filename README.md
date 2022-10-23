# Examples

Somethings to show in video

## List

- pandoc with no css

  ```shell
  pandoc -s leaf1.md -o leaf1.html
  ```

- pandoc with custom css

  ```shell
  pandoc -s leaf1.md -c pandoc.css -o leaf1-2.html
  ```

- Single page with mkdocs - example 1

  ```shell
  mkdocs serve
  ```

- Single page with styling - example 2

  ```shell
  mkdocs serve
  ```

- full site with styling and additional plugin - example 3

  ```shell
  mkdocs serve
  ```

- build site for offline viewing

  ```shell
  mkdocs build
  ```

- host created site with containers

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
- [AVD and Docs running on Docker or Kubernetes by Thomas G](https://github.com/titom73/demo-avd-compose-k8s)
