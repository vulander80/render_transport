FROM node:18-alpine

WORKDIR /app

# Copy only package.json first for better caching
COPY package*.json ./

COPY . .
# Install dependencies
RUN npm install

# Copy the rest of the app code


EXPOSE 3000

CMD ["npm", "start", "--verbose"]