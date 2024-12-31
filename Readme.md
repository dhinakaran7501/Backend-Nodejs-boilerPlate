
  <h1 style="color: #007acc; text-align: center;">Backend Node.js Boilerplate</h1>
  <h3 style="color: #007acc; text-align: center;">
    <span style="display: inline-block; background-color: #007acc; color: white; padding: 5px 10px; border-radius: 5px; font-size: 14px;">
      Scalable & Modern Backend Starter
    </span>
  </h3>

  <p>
    Welcome to the <strong>Backend Node.js Boilerplate</strong>! This project is a 
    fully-configured starter template designed for rapid backend development with 
    <strong>TypeScript</strong>, <strong>ESLint</strong>, <strong>Prettier</strong>, and more.
  </p>

  <h2 style="color: #007acc;">🔧 Features</h2>
  <ul style="margin: 10px 0; padding-left: 20px;">
    <li>Pre-configured <strong>TypeScript</strong> for type safety.</li>
    <li>Linting and formatting with <strong>ESLint</strong> and <strong>Prettier</strong>.</li>
    <li>Structured logging using <strong>Winston</strong>.</li>
    <li>Reusable Cron Job Functions.</li>
    <li>Scalable folder structure for easy project management.</li>
  </ul>

  <h2 style="color: #007acc;">📁 Project Structure</h2>
  <pre style="background-color: #f4f4f4; padding: 10px; border-radius: 5px; overflow-x: auto;">
src/
├── config/         # Environment configurations and database connections.
├── controllers/    # API response handling and messaging logic.
├── routes/         # Route definitions with multiple path support.
├── services/       # Business logic and database interactions.
├── types/          # TypeScript type definitions for various components.
├── utils/          # Helper functions and utilities.
│   ├── helper.ts   # Reusable functions.
│   └── logger.ts   # Configured Winston logger for structured logging.
├── server.ts       # The entry point of the application.
  </pre>

  <h2 style="color: #007acc;">⚙️ Setup and Installation</h2>
  <ol style="margin: 10px 0; padding-left: 20px;">
    <li><strong>Clone the Repository:</strong>
      <pre style="background-color: #f4f4f4; padding: 10px; border-radius: 5px; overflow-x: auto;">git clone https://github.com/dhinakaran7501/Backend-Nodejs-boilerPlate.git</pre>
    </li>
    <li><strong>Install Dependencies:</strong>
      <pre style="background-color: #f4f4f4; padding: 10px; border-radius: 5px; overflow-x: auto;">npm install</pre>
    </li>
    <li><strong>Create a `.env` File:</strong>
      <pre style="background-color: #f4f4f4; padding: 10px; border-radius: 5px; overflow-x: auto;">
PORT=3000
DATABASE_URL=your_database_url
JWT_SECRET=your_secret_key
      </pre>
    </li>
    <li><strong>Start the Development Server:</strong>
      <pre style="background-color: #f4f4f4; padding: 10px; border-radius: 5px; overflow-x: auto;">npm run dev</pre>
    </li>
  </ol>

  <h2 style="color: #007acc;">⏲ Cron Job Timer Format</h2>
  <pre style="background-color: #f4f4f4; padding: 10px; border-radius: 5px; overflow-x: auto;">
┌───────────── Minute (0 - 59)
│ ┌───────────── Hour (0 - 23)
│ │ ┌───────────── Day of Month (1 - 31)
│ │ │ ┌───────────── Month (1 - 12)
│ │ │ │ ┌───────────── Day of Week (0 - 6) (Sunday = 0)
* * * * *
  </pre>
  <p>Examples:</p>
  <table style="border-collapse: collapse; width: 100%; margin: 20px 0;">
    <thead>
      <tr>
        <th style="border: 1px solid #ddd; padding: 8px; background-color: #007acc; color: white;">Cron Expression</th>
        <th style="border: 1px solid #ddd; padding: 8px; background-color: #007acc; color: white;">Description</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px;">0 0 * * *</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Run at midnight every day.</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px;">*/5 * * * *</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Run every 5 minutes.</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px;">0 9 * * 1</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Run at 9:00 AM every Monday.</td>
      </tr>
    </tbody>
  </table>

  <h2 style="color: #007acc;">👨‍💻 Author</h2>
  <p><strong>Dhinakaran R</strong></p>
  <p>
    LinkedIn: <a href="https://linkedin.com/in/dhinakaran7501" style="color: #007acc;">Dhinakaran R</a><br>
    GitHub: <a href="https://github.com/dhinakaran7501" style="color: #007acc;">@dhinakaran7501</a>
  </p>
