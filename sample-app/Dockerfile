# Use official lightweight Node image
FROM node:18-alpine

# Create app dir
WORKDIR /usr/src/app

# Copy package.json (no deps here but best practice)
COPY package.json ./

# Install dependencies (none in this minimal example)
RUN npm install --production

# Copy app source
COPY app.js ./

# Expose port
EXPOSE 5000

# Start the app
CMD ["node", "app.js"]

