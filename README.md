# Next.js Prisma SQLite Starter

This is a starter project combining Next.js with Prisma and SQLite. It provides a foundational setup for building a modern web application with a focus on database-backed features using Prisma ORM and SQLite as the database.

## Features

- **Next.js 14.1.4**: For server-side rendering, API routes, and fast front-end development.
- **Prisma ORM**: Simplifies database interactions with an intuitive schema and type-safe queries.
- **SQLite**: Lightweight database for quick development setups and small-scale projects.
- **Tailwind CSS**: Utility-first CSS framework for styling.
- **TypeScript**: Enhances development with type safety.

## Prerequisites

Before starting, ensure you have the following installed:

- Node.js (v16 or later recommended)
- npm or yarn

## Getting Started

### 1. Clone the Repository
```bash
git clone <repository-url>
cd nextjs-prisma-sqlite
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Set Up Prisma
Run the following command to initialize Prisma and create your SQLite database:
```bash
npx prisma db push
```

If you have seed data, run the seed script:
```bash
npm run prisma-seed
```

### 4. Run the Development Server
Start the Next.js development server:
```bash
npm run dev
```

Navigate to [http://localhost:3000](http://localhost:3000) in your browser to see your app.

## Scripts

The following scripts are defined in the `package.json` file:

- **`npm run dev`**: Starts the development server.
- **`npm run build`**: Builds the project for production.
- **`npm run start`**: Starts the production server.
- **`npm run lint`**: Lints the code using ESLint.
- **`npm run prisma-seed`**: Runs the Prisma seed script located in `prisma/seed.ts`.

## Project Structure

- **`pages/`**: Contains Next.js pages.
- **`prisma/`**: Contains the Prisma schema (`schema.prisma`) and seed script (`seed.ts`).
- **`styles/`**: Contains global and component-specific styles.

## Dependencies

### Main Dependencies

- `@prisma/client`: Client library for Prisma ORM.
- `next`: Framework for server-side rendering and static site generation.
- `react` and `react-dom`: Core libraries for building user interfaces.
- `sqlite3`: SQLite database driver.

### Development Dependencies

- `typescript`: Type safety.
- `tsx`: TypeScript execution framework.
- `tailwindcss` and `postcss`: For styling.
- `eslint` and `eslint-config-next`: For linting and code quality.
- `@types/react` and `@types/react-dom`: TypeScript definitions for React.
- `@types/node`: TypeScript definitions for Node.js.

## Styling

This project uses Tailwind CSS for styling. You can customize the configuration in the `tailwind.config.js` file.

## Prisma

Prisma is set up with SQLite as the database. Update the `prisma/schema.prisma` file to define your database models. After making changes to the schema, run:

```bash
npx prisma db push
```

## Contributing

Contributions are welcome! Please submit a pull request or raise an issue if you have suggestions or bug reports.

## License

This project is licensed under [MIT License](LICENSE).

