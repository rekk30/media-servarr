# media-servarr
Media server using *arr stack and docker-compose.

```console
docker-compose up -d
```

### Prowlarr Postgresql
Create two databases:

- **prowlarr-main** For configuration and history
- **prowlarr-log** For logs

Add to the Prowlarr `config.xml`:
```xml
<PostgresUser>postgres user</PostgresUser>
<PostgresPassword>postgres pass</PostgresPassword>
<PostgresPort>postgres port</PostgresPort>
<PostgresHost>postgres hostname</PostgresHost>
```
You can also specify a databases name
```xml
<PostgresMainDb>main db name</PostgresMainDb>
<PostgresLogDb>log db name</PostgresLogDb>
```
### Radarr Postgresql
Create two databases:

- **radarr-main** For configuration and history
- **radarr-log** For logs

Add to the Radarr `config.xml`:
```xml
<PostgresUser>postgres user</PostgresUser>
<PostgresPassword>postgres pass</PostgresPassword>
<PostgresPort>postgres port</PostgresPort>
<PostgresHost>postgres hostname</PostgresHost>
```
You can also specify a databases name
```xml
<PostgresMainDb>main db name</PostgresMainDb>
<PostgresLogDb>log db name</PostgresLogDb>
```

