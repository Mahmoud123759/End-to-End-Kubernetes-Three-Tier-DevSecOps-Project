FROM node:18
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
COPY . .
# Create non-root user
RUN useradd -m appuser
USER appuser
CMD ["node", "index.js"] 
