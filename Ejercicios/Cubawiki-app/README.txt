# Ejercicio: Completar configuración de `docker-compose.yml`

Se te entrega un archivo `docker-compose.yml` parcialmente incompleto que define una arquitectura de **3 servicios**:  

1. **Base de datos (PostgreSQL)**  
   - Debe escuchar en el puerto **5432** (interno del contenedor).  
   - El volumen `postgres_data` ya está creado para persistencia.  

2. **Backend (Flask)**  
   - Debe levantar en el puerto **5000**.  
   - Ya está configurado para esperar a que la base de datos esté lista antes de iniciar.  

3. **Frontend (React con Vite)**  
   - Debe levantar en el puerto **5173**.  

Además, todos los servicios deben estar conectados a una **red interna compartida** para que puedan comunicarse entre sí.  

---

## Tareas

1. Completar las secciones `ports:` de cada servicio para que sean accesibles desde la máquina host.  

2. Definir una red personalizada y conectar **todos los servicios** a esa red.  

3. Verificar que levantar los contenedores con:

   ```bash
   docker compose up