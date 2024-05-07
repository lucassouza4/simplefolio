# Usa uma imagem Node.js como base
FROM node:latest

# Define o diretório de trabalho dentro do contêiner
WORKDIR /app

# Copia os arquivos package.json e package-lock.json para o diretório de trabalho
COPY package*.json ./

# Instala as dependências do projeto
RUN npm install

# Copia todo o código-fonte para o diretório de trabalho
COPY . .

# Expõe a porta 1234, que é a porta padrão para o servidor de desenvolvimento do Parcel
EXPOSE 1234

# Comando para iniciar a aplicação
CMD ["npm", "start"]
