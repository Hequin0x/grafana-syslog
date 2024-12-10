# Grafana Syslog

This is a docker-compose project that uses Grafana, Loki and Alloy to receive and display syslog data.

## Configuration

The configuration is done in the `docker-compose.yml` file. The following environment variables are available:
- `MINIO_ROOT_USER` - The username for the Minio server.
- `MINIO_ROOT_PASSWORD` - The password for the Minio server.
- `LOKI_PATH_PREFIX` - The path prefix for the Loki server.
- `LOKI_S3_DATA_BUCKET_NAME` - The name of the data bucket for the Loki server.
- `LOKI_S3_RULER_BUCKET_NAME` - The name of the ruler bucket for the Loki server.
- `LOKI_COMPACTOR_WORKING_DIR` - The working directory for the Loki compactor.
- `LOKI_COMPACTOR_RETENTION_ENABLED` - Whether the retention is enabled for the Loki compactor.
- `LOKI_COMPACTOR_RETENTION_PERIOD` - The retention period for the Loki compactor.
- `GF_AUTH_ANONYMOUS_ENABLED` - Whether the anonymous authentication is enabled for Grafana.
