# Kafka Backend

This is the backend part of the Kafka plugin. It responds to Kafka requests from the frontend.

## Configuration

This configures how to connect to the brokers in your Kafka cluster.

### clientId

The name of the client to use when connecting to the cluster.

### brokers

A list of the brokers' host names and ports to connect to.

### SSL (optional)

Configure TLS connection to the Kafka cluster. The options are passed directly to [tls.connect] and used to create the TLS secure context. Normally these would include `key` and `cert`.

Example:

```yaml
kafka:
  clientId: backstage
  brokers:
    - localhost:9092
```
