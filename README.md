docker-bookdown
===============

[![pulls-badge]][docker-hub]
[![automated-build-badge]][docker-hub]

A docker image with everything needed to compile bookdown projects (including
PDF support).

Usage
-----

    $ docker run \
      -it \
      -v $(pwd)/book:/book
      0xcaff/bookdown bash

    (inside container) $ cd book
    (inside container) $ Rscript -e "bookdown::render_book('.', 'all')"

[automated-build-badge]: https://img.shields.io/docker/automated/0xcaff/bookdown.svg
[pulls-badge]: https://img.shields.io/docker/pulls/0xcaff/bookdown.svg
[docker-hub]: https://hub.docker.com/r/0xcaff/bookdown/
