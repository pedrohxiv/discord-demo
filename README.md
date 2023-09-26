# Projeto Demo Discord

## Descrição do Projeto

O Discord Demo é uma plataforma de demonstração que simula funcionalidades do Discord, uma popular plataforma de comunicação por voz, vídeo e texto para comunidades online. Este projeto demonstra algumas das principais funcionalidades do Discord, como bate-papo por texto, bate-papo por voz e video, envio de arquivos, emojis e muito mais. É uma demonstração interativa para explorar como o Discord funciona.

## Funcionalidades

### 1. Bate-Papo por Texto

O Discord Demo permite que os usuários participem de bate-papos por texto em tempo real. Eles podem criar servidores, canais e trocar mensagens com outros usuários. A biblioteca `socket.io` versão `^4.7.2` é utilizada para a comunicação em tempo real.

### 2. Bate-Papo por Voz e Vídeo

Os usuários também podem participar de bate-papos por voz, onde podem se conectar a canais de voz, conversar com outros usuários e compartilhar suas experiências. Isso é possível graças ao uso do `livekit-client` versão `^1.13.2`.

### 3. Envio de Arquivos

É possível enviar arquivos, como imagens e documentos, em mensagens de bate-papo. A funcionalidade de envio de arquivos é implementada com a ajuda da biblioteca `uploadthing` versão `^5.5.2`.

### 4. Emojis

O Discord Demo oferece suporte a emojis para enriquecer as conversas. Ele utiliza a biblioteca `emoji-mart` versão `^5.5.2` para fornecer uma ampla seleção de emojis.

### 5. Integração com UploadThing

A plataforma integra-se ao UploadThing, permitindo que os usuários façam upload e compartilhem arquivos de forma simples e rápida. As chaves `UPLOADTHING_SECRET` e `UPLOADTHING_APP_ID` são configuradas para habilitar essa integração.

## Dependências

A seguir estão as principais dependências utilizadas no desenvolvimento do projeto:

- `@clerk/nextjs` v4.23.3
- `@emoji-mart/data` v1.1.2
- `@emoji-mart/react` v1.1.1
- `@hookform/resolvers` v3.3.1
- `@livekit/components-react` v1.1.8
- `@livekit/components-styles` v1.0.6
- `@prisma/client` v5.2.0
- `@radix-ui/react-avatar` v1.0.3
- `@radix-ui/react-dialog` v1.0.4
- `@radix-ui/react-dropdown-menu` v2.0.5
- `@radix-ui/react-label` v2.0.2
- `@radix-ui/react-popover` v1.0.6
- `@radix-ui/react-scroll-area` v1.0.4
- `@radix-ui/react-select` v1.2.2
- `@radix-ui/react-separator` v1.0.3
- `@radix-ui/react-slot` v1.0.2
- `@radix-ui/react-tooltip` v1.0.6
- `@tanstack/react-query` v4.35.0
- `@types/node` v20.5.9
- `@types/react` v18.2.21
- `@types/react-dom` v18.2.7
- `@types/uuid` v9.0.3
- `@uploadthing/react` v5.5.0
- `autoprefixer` v10.4.15
- `axios` v1.5.0
- `class-variance-authority` v0.7.0
- `clsx` v2.0.0
- `cmdk` v0.2.0
- `date-fns` v2.30.0
- `emoji-mart` v5.5.2
- `eslint` v8.48.0
- `eslint-config-next` v13.4.12
- `livekit-client` v1.13.2
- `livekit-server-sdk` v1.2.6
- `lucide-react` v0.274.0
- `next` v13.4.12
- `next-themes` v0.2.1
- `postcss` v8.4.29
- `prisma` v5.2.0
- `query-string` v8.1.0
- `react` v18.2.0
- `react-dom` v18.2.0
- `react-dropzone` v14.2.3
- `react-hook-form` v7.46.1
- `socket.io` v4.7.2
- `socket.io-client` v4.7.2
- `tailwind-merge` v1.14.0
- `tailwindcss` v3.3.3
- `tailwindcss-animate` v1.0.7
- `typescript` v5.2.2
- `uploadthing` v5.5.2
- `uuid` v9.0.0
- `zod` v3.22.2
- `zustand` v4.4.1

## Como Executar o Projeto

1. Clone este repositório em sua máquina local.
2. Certifique-se de ter o Node.js e o npm (ou yarn) instalados.
3. Instale as dependências do projeto utilizando o seguinte comando:

```bash
npm install
# ou
yarn install
```

4. Crie um arquivo `.env` na raiz do projeto com as seguintes chaves e seus respectivos valores:

```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=seu_valor_aqui
CLERK_SECRET_KEY=seu_valor_aqui
NEXT_PUBLIC_CLERK_SIGN_IN_URL=seu_valor_aqui
NEXT_PUBLIC_CLERK_SIGN_UP_URL=seu_valor_aqui
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=seu_valor_aqui
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=seu_valor_aqui
DATABASE_URL=seu_valor_aqui
UPLOADTHING_SECRET=seu_valor_aqui
UPLOADTHING_APP_ID=seu_valor_aqui
LIVEKIT_API_KEY=seu_valor_aqui
LIVEKIT_API_SECRET=seu_valor_aqui
NEXT_PUBLIC_LIVEKIT_URL=seu_valor_aqui
```

Certifique-se de substituir `seu_valor_aqui` pelos valores corretos de cada chave.

5. Para iniciar o servidor de desenvolvimento, utilize o seguinte comando:

```bash
npm run dev
# ou
yarn dev
```

6. O projeto estará disponível em `http://localhost:3000`.
