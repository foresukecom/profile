FROM ubuntu:latest

# Install necessary packages
RUN apt-get update && apt-get install -y curl git vim zsh sudo locales tree imagemagick

# Set locale to Japanese
RUN locale-gen ja_JP.UTF-8
ENV LANG ja_JP.UTF-8
ENV LANGUAGE ja_JP:ja
ENV LC_ALL ja_JP.UTF-8

# Set working directory
WORKDIR /workspace

# Set default command
CMD [ "/bin/zsh" ]
