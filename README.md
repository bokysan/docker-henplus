This is a docker image to run the HenPlus (https://github.com/neurolabs/henplus) JDBC tool inside Docker (https://www.docker.com/).

The image already includes the PostgreSQL JDBC driver. If you need
additional drivers, add them to the `jdbc` directory.

=== Usage ===

To use this just run the docker image with:

```bash
  docker run --rm boky/henplus --help
```

e.g. to connect to a database in your swarm, you would do something like this:

```bash
  docker run --net=swarm_db -it --rm boky/henplus -J jdbc:postgresql://database/sample -U sample -P demopassword
```
