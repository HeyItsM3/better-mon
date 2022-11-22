# Which Pokémon is better?

##  Getting Started

Prerequisite:

- MySQL local database (or Planetscale connection using PScale CLI)
- npm

Setup

1. Clone repository
1. `npm install`
1. Create `.env` file if one does not already exist
1. Add connection URLs for both database and shadow db to .env ([example .env file here](https://gist.github.com/TheoBr/e450c52a52a9f9c9b49ef07212689685))
1. If you're using planetscale:
- First connect to database on the terminal if your using PScale CLI ([here its how to install it](https://github.com/planetscale/cli)).
- Then you must run `pscale connect "yourDbName" main --port 3309`
- And in another terminal `pscale connect "yourDbShadowNAME" main-shadow --port 3312`
6. Initialize database - `npx prisma migrate dev`
7. Initialize base data set - `npm run ts-node ./scripts/fill-db.ts`
8. Run dev server `npm run dev`

Tech stack:

1. tRCP: https://trpc.io/
1. PlanetScale: https://planetscale.com/
1. Prisma: https://www.prisma.io/
1. Next.js: https://nextjs.org/
1. Tailwind: https://tailwindcss.com/

[More info](https://www.twitch.tv/theo)
