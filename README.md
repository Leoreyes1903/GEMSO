# GEMSO - Equipo B

## Autores

- Equipo B  
- Grupo 101  

---

## Instrucciones de uso

1. Crea un archivo `.env` en la raíz del proyecto.  
   Puedes basarte en el archivo `.env.example` para saber qué variables necesitas.

2. Instala las dependencias con tu gestor de paquetes favorito:
   ```
   npm i
   
   ```   

3. Para saber los comandos disponibles, revisa esta sección o abre el archivo `package.json`.

---

## Comandos disponibles

Estos son los scripts definidos en el `package.json` para facilitar el desarrollo y despliegue:

| Comando            | Descripción |
|--------------------|-------------|
| `dev`              | Inicia el servidor de desarrollo con Turbo (Next.js App Router). |
| `build`            | Compila la aplicación para producción. |
| `preview`          | Construye y arranca la app como si estuviera en producción. |
| `start`            | Inicia la aplicación construida desde `.next`. |
| `typecheck`        | Verifica los tipos de TypeScript sin emitir archivos. |
| `check`            | Linter y formateador del proyecto con [Biome](https://biomejs.dev/). |
| `check:write`      | Aplica correcciones automáticas de formato con Biome. |
| `check:unsafe`     | Aplica correcciones incluso las que podrían cambiar el comportamiento. |
| `db:see` / `db:studio` | Abre Prisma Studio en el navegador para editar y visualizar la base de datos. |
| `db:generate`      | Ejecuta migraciones locales (`prisma migrate dev`) y actualiza el cliente Prisma. |
| `db:migrate`       | Aplica migraciones pendientes en producción (`prisma migrate deploy`). |
| `db:push`          | Fuerza la sincronización de la base de datos con el esquema (`prisma db push`). Solo para desarrollo. |
| `postinstall`      | Ejecuta `prisma generate` automáticamente después de instalar dependencias. |

---

## Estructura del proyecto (resumen)

```

/prisma          → Esquema de Prisma y migraciones
/public          → Archivos estáticos
/src             → Código fuente compartido (env, utils, app, server(App Routing))
/node_modules    → Dependencias (no se sube al repo, pero se genera cuando instalas las dependencias)
.env             → Variables de entorno (no se sube al repo)
```

---