# Como a aplicacao é node é necessário uma imagem base node para que a aplicacao funcione
FROM node:16.15.0
# Definir um diretório de trabalho, onde vai jogar os arquivos de execucao na pasta para poder utilizalos
WORKDIR /app
# Baixar\Copiar os pacotes para depois realizar a execucao(Pacotes já inclusos no projeto)
COPY ./package*.json ./
# npm é o gerenciador de pacotes do node e se torna necessário para execucao dos pacotes
RUN npm install
# Copia o restante dos arquivos.
COPY . .
##Definindo\expondo a porta 8080 da aplicacao.
EXPOSE 8080
# Iniciar a aplicacao
CMD ["node","server.js"]
