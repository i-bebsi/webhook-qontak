FROM mcr.microsoft.com/vscode/devcontainers/php:8.3

# system deps
RUN apt-get update && apt-get install -y git unzip libzip-dev curl openssl

# nodejs
RUN curl -fsSL https://deb.nodesource.com/setup_18.x | bash - && apt-get install -y nodejs

# php extensions
RUN docker-php-ext-install pdo_mysql zip

ENV PATH="${PATH}:/root/.composer/vendor/bin"
