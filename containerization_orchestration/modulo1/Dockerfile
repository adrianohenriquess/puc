FROM ubuntu:22.04
LABEL maintainer=adriano.henriquesds@gmail.com.br
COPY . /var/www/html
EXPOSE 8080
RUN apt-get update -y && apt-get install --no-install-recommends python3 -y
WORKDIR /var/www/html
ENTRYPOINT ["python3", "-m", "http.server", "8080"]
