FROM node:14
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
# Create non-root user
RUN useradd -m appuser
USER appuser

COPY . .
CMD ["node", "index.js"]
