# prisma-server

# Detener Prisma
docker-compose stop

# Iniciar Prisma
docker-compose up -d

# Para aplicar los cambios que acaba de realizar en el modelo de datos. (datamodel.prisma)
HTTP:  http://localhost:4466
WS:    ws://localhost:4466
prisma deploy

# Regenerar el cliente Prisma
# Debido a que el cliente Prisma se basa en el modelo de datos, debe regenerarse cada vez que se actualice el modelo de datos. (/generated/prisma)
prisma generate

# Para generar o actualizar el modelo de datos realizando una instrospección del esquema de base de datos.
prisma introspect

