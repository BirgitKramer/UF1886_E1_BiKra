# Versiones por entornos (DEV / QA / PROD)

## Comandos utilizados

### Odoo
- `sudo docker exec -it odoo-dev odoo --version`
- `sudo docker exec -it odoo-qa odoo --version`
- `sudo docker exec -it odoo-prod odoo --version`

### PostgreSQL
- `sudo docker exec -it postgres-qa postgres --version`
- `sudo docker exec -it postgres-dev postgres --version`
- `sudo docker exec -it postgres-prod postgres --version`

#### Apache Hop
- Imagen detectada por `Docker ps -a`: `apache/hop:latest` 
- `sudo docker exec -it hop-dev /cpt/hop/hop-config.sh -v`
- `sudo docker exec -it hop-qa /cpt/hop/hop-config.sh -v`
- `sudo docker exec -it hop-prod /cpt/hop/hop-config.sh -v`

## Tabla de versiones
| Entorno | Odoo | PostgreSQL | Hop |
|---|---|---|---|
| DEV | Odoo Server 18.0-20251222 | postgres (PostgreSQL) 16.11 | apache/hop:latest |
| QA | Odoo Server 18.0-20251222 | postgres (PostgreSQL) 16.11 | apache/hop:latest |
| PROD | Odoo Server 18.0-20251222 | postgres (PostgreSQL) 16.11 | apache/hop:latest |

## Observaciones
- Odoo y  PostgreSQL estan alineados en los tres entornos (misma version)
- Hop tambien esta alineado por el tag de la imagen (`2.17.0`). 

