FROM redis:latest

# Environment varibales
# REDIS_PORT
# REDIS_PASSWORD

ENV REDIS_PORT=${REDIS_PORT:-6379}

EXPOSE ${REDIS_PORT}

# Entry point
CMD ["sh", "-c", "redis-server --port ${REDIS_PORT} ${REDIS_PASSWORD:+--requirepass} ${REDIS_PASSWORD}" ]
