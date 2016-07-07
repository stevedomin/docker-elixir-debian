FROM stevedomin/erlang:18.2
MAINTAINER Steve Domin <steve@stevedomin.com>

RUN apt-get update && \
  apt-get install locales && \
  echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen && \
  locale-gen

ENV LC_ALL="en_US.UTF-8"

RUN apt-get update && apt-get install -y \
  elixir=1.3.1-1

CMD ["iex"]
