FROM elixir:1.14-otp-25-slim

WORKDIR /app
COPY . /app

ARG MIX_ENV=prod
RUN mix release

CMD ["_build/prod/rel/greeter/bin/greeter", "start"]
