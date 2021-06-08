From node:14-alpine
RUN apk add --no-cache git
RUN npm install --force -g npx create-nuxt-app
WORKDIR /src
CMD ["create-nuxt-app", "blog"]
