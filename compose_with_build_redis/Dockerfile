FROM redis:6.2

WORKDIR /app

RUN adduser --system --group --disabled-password --gecos '' user

RUN mkdir /conf && touch /conf/redis.conf

RUN chown -R user:user /conf

CMD ["redis-server /conf/redis.conf"]