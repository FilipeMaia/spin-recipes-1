# postgres-root

This recipe shows a working example of Postgres on Spin using the official managed image.

Features of this recipe:
  * Persistent storage on Rancher NFS.
  * Login credentials on Rancher Secrets.
  * Optional direct access vi SQL monitor from within NERSC networks.
  * Custom configuration options supplied through runtime arguments, avoiding the
    need to create (and maintain) a custom image.
  * Health checking and automatic reschedulig in the event of problems.
  * Enhanced security through a reduced set of capabilities.

To use this recipe, incorporate it into your `docker-compose.yml` and `rancher-compose.yml`,
substituting the name of your stack for `postgres-root` and the database username of your choice.