ARG NODE_VERSION=20
ARG PLAYWRIGHT_VERSION=1.44.0
ARG PNPM_VERSION=8.15.7

FROM node:${NODE_VERSION}

RUN npx -y playwright@${PLAYWRIGHT_VERSION} install --with-deps

RUN npm install -g pnpm@${PNPM_VERSION}
RUN pnpm config set store-dir ~/.pnpm-store
RUN pnpm config set verify-store-integrity false
