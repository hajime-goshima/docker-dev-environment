FROM ruby:3

# Prepare install nodejs
RUN mkdir -p /etc/apt/keyrings
RUN curl -fsSL https://deb.nodesource.com/gpgkey/nodesource-repo.gpg.key | gpg --dearmor -o /etc/apt/keyrings/nodesource.gpg
RUN echo "deb [signed-by=/etc/apt/keyrings/nodesource.gpg] https://deb.nodesource.com/node_20.x nodistro main" | tee /etc/apt/sources.list.d/nodesource.list

# Install packages
RUN apt-get update -qq
RUN apt-get install -y ca-certificates curl gnupg vim default-mysql-client nodejs redis-tools

# Enable yarn with corepack
RUN corepack enable

WORKDIR /app

#COPY Gemfile /myapp/Gemfile
#COPY Gemfile.lock /myapp/Gemfile.lock
#RUN bundle install

ENTRYPOINT ["sleep", "infinity"]