# Use Node.js 18 (LTS) instead of 14
FROM node:18-alpine 

WORKDIR /usr/src/app

COPY package*.json ./

# Install dependencies (use --omit=dev for production)
RUN npm install --omit=dev

COPY . .

# Ensure this matches your backend's actual port (e.g., 5000 or 8000)
EXPOSE 8000  

# Start the app (replace "index.js" if your entry file is different)
CMD ["node", "index.js"]