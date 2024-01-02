# Use the official PostgreSQL image as a base image
FROM postgres:latest

# Environment variables to configure the PostgreSQL database
ENV POSTGRES_USER="admin"
ENV POSTGRES_HOST="localhost"
ENV POSTGRES_PASSWORD="admin"
ENV POSTGRES_DATABASE="nextjs_dashboard_postgres"

# Expose the default PostgreSQL port
EXPOSE 5432

# Copy the initialization script to the container
COPY ./docker/nextjs-dashboard-postgres/init.sql /docker-entrypoint-initdb.d/

# Optionally, you can include additional scripts
# COPY other_init_script.sql /docker-entrypoint-initdb.d/

# The CMD instruction specifies the command to run on container startup
# CMD ["postgres"]