# gemini-cli-webui

This project aims to provide a web-based user interface for the `gemini-cli`.

It is implemented using the [T3 Stack](https://create.t3.gg/) and will start with a minimal viable implementation, adhering to the YAGNI principle.

## Technologies Used

- [Next.js](https://nextjs.org)
- [NextAuth.js](https://next-auth.js.org)
- [Prisma](https://prisma.io)
- [Drizzle](https://orm.drizzle.team)
- [Tailwind CSS](https://tailwindcss.com)
- [tRPC](https://trpc.io)

## Getting Started

1.  Clone the repository:
    ```bash
    git clone https://github.com/Grac11111aq/gemini-cli-webui.git
    cd gemini-cli-webui
    ```
2.  Install dependencies:
    ```bash
    npm install
    ```
3.  Set up environment variables:
    Copy `.env.example` to `.env` and fill in the required values. For initial development, you can set `AUTH_SECRET` to any string and leave `AUTH_DISCORD_ID` and `AUTH_DISCORD_SECRET` empty (they are made optional in `src/env.js` for development).
    ```bash
    cp .env.example .env
    ```
4.  Start the development server:
    ```bash
    npm run dev
    ```
    The application will be accessible at `http://localhost:3000`.

## Project Scope

This project focuses on providing a web interface to interact with the `gemini-cli`. The initial implementation will be kept as minimal as possible, adding features incrementally as needed.

## Contributing

Contributions are welcome! Please feel free to open issues or submit pull requests.