FROM redis:7.0.8-alpine

# Environment varibales
# REDIS_PORT
# REDIS_PASSWORD

ENV REDIS_PORT=${REDIS_PORT:-6379}

EXPOSE ${REDIS_PORT}

# Entry point
CMD ["sh", "-c", "redis-server --port ${REDIS_PORT} --save '' ${REDIS_PASSWORD:+--requirepass} ${REDIS_PASSWORD}" ]
