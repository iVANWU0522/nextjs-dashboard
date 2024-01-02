# Docker
Run the nestjs app in docker container
```
# Build the image
docker --context orbstack build --no-cache -t nextjs-dashboard-app -f ./docker/nextjs-dashboard-app/Dockerfile .

# Run the container
docker --context orbstack run -d --name nextjs-dashboard-app -p 3000:3000 nextjs-dashboard-app
```

Run the postgres db in docker container
```
# Build the image
docker --context orbstack build --no-cache -t nextjs-dashboard-postgres -f ./docker/nextjs-dashboard-postgres/Dockerfile .

# Run the container
docker --context orbstack run -d --name nextjs-dashboard-postgres -p 5432:5432 nextjs-dashboard-postgres
```