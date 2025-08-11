# Producto-2-Base-de-Datos-No-Relacional-MongoDB-
Implementación de protocolos para gestión de bases de datos no relacionales, incluyendo respaldos, seguridad y automatización con Python.
## Tecnologías
- MongoDB 7.0+
- Python 3.x (PyMongo)
- MongoDB Compass

## Estructura
/Scripts
├── respaldo.py # Copias de seguridad
├── actualizacion.py # Procesos por lotes
/Backups
├── backup_YYYYMMDD.json # Ejemplo

## Instalación
1. Configurar autenticación en `mongod.cfg`:
   ```yaml
   security:
     authorization: enabled
   Crear usuarios:
   db.createUser({user: "admin", roles: ["root"]});
## Uso
  Respaldo binario:
  mongodump --db BAJASUR --out /backups
## Monitoreo:
  mongostat --host localhost
## Documentación
