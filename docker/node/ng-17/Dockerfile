FROM node:20-bullseye-slim

# Actualizar paquetes e instalar dependencias necesarias
RUN apt-get update && apt-get install -y \
    git \
    libc6-dev \
    fonts-noto-color-emoji \
    vim \
    && rm -rf /var/lib/apt/lists/*  # Limpiar caché de paquetes para reducir el tamaño de la imagen

# Instalar Angular CLI 17
RUN npm install -g @angular/cli@17

# Configurar locales para soporte de caracteres Unicode
ENV LANG=C.UTF-8
ENV LC_ALL=C.UTF-8
