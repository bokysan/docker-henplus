This is a docker image to run the HenPlus (https://github.com/neurolabs/henplus) JDBC tool inside Docker (https://www.docker.com/).

The image already includes the PostgreSQL JDBC driver. If you need
additional drivers, add them to the `jdbc` directory.

=== Usage ===

To use this just run the docker image with:

```bash
  docker run -rm -it boky/henplus /usr/share/henplus
```
