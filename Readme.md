<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Backend Node.js Boilerplate</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 20px;
      color: #333;
    }
    h1, h2, h3 {
      color: #007acc;
      text-align: center;
    }
    h1 {
      margin-bottom: 10px;
    }
    .badge {
      display: inline-block;
      background-color: #007acc;
      color: white;
      padding: 5px 10px;
      border-radius: 5px;
      font-size: 14px;
    }
    pre, code {
      background-color: #f4f4f4;
      padding: 10px;
      border-radius: 5px;
      overflow-x: auto;
      position: relative;
    }
    pre button {
      position: absolute;
      top: 10px;
      right: 10px;
      background-color: #007acc;
      color: white;
      border: none;
      padding: 5px 10px;
      border-radius: 5px;
      cursor: pointer;
    }
    pre button:hover {
      background-color: #005b9f;
    }
    ul, ol {
      margin: 10px 0;
      padding-left: 20px;
    }
    li {
      margin-bottom: 5px;
    }
    .table {
      border-collapse: collapse;
      width: 100%;
      margin: 20px 0;
    }
    .table th, .table td {
      border: 1px solid #ddd;
      padding: 8px;
      text-align: left;
    }
    .table th {
      background-color: #007acc;
      color: white;
    }
    a {
      color: #007acc;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    .center {
      text-align: center;
    }
    .copy-message {
      color: green;
      font-size: 14px;
      margin-top: 5px;
      text-align: center;
    }
  </style>
  <script>
    function copyToClipboard(text) {
      navigator.clipboard.writeText(text).then(() => {
        const message = document.getElementById("copy-message");
        message.style.display = "block";
        setTimeout(() => {
          message.style.display = "none";
        }, 2000);
      });
    }
  </script>
</head>
<body>
  <h1 style="color: #007acc;">Backend Node.js Boilerplate</h1>
  <h3><span class="badge">Scalable & Modern Backend Starter</span></h3>

  <p>
    Welcome to the <strong>Backend Node.js Boilerplate</strong>! This project is a 
    fully-configured starter template designed for rapid backend development with 
    <strong>TypeScript</strong>, <strong>ESLint</strong>, <strong>Prettier</strong>, and more.
  </p>

  <h2>🔧 Features</h2>
  <ul>
    <li>Pre-configured <strong>TypeScript</strong> for type safety.</li>
    <li>Linting and formatting with <strong>ESLint</strong> and <strong>Prettier</strong>.</li>
    <li>Structured logging using <strong>Winston</strong>.</li>
    <li>Reusable Cron Job Functions.</li>
    <li>Scalable folder structure for easy project management.</li>
  </ul>

  <h2>📁 Project Structure</h2>
  <pre>
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

  <h2>⚙️ Setup and Installation</h2>
  <ol>
    <li><strong>Clone the Repository:</strong>
      <pre>
git clone https://github.com/dhinakaran7501/Backend-Nodejs-boilerPlate.git
<button onclick="copyToClipboard('git clone https://github.com/dhinakaran7501/Backend-Nodejs-boilerPlate.git')">Copy</button>
      </pre>
      <div id="copy-message" class="copy-message" style="display: none;">Link copied to clipboard!</div>
    </li>
    <li><strong>Install Dependencies:</strong>
      <pre>
npm install
<button onclick="copyToClipboard('npm install')">Copy</button>
      </pre>
    </li>
    <li><strong>Create a `.env` File:</strong>
      <pre>
PORT=3000
DATABASE_URL=your_database_url
JWT_SECRET=your_secret_key
      <button onclick="copyToClipboard('PORT=3000\nDATABASE_URL=your_database_url\nJWT_SECRET=your_secret_key')">Copy</button>
      </pre>
    </li>
    <li><strong>Start the Development Server:</strong>
      <pre>
npm run dev
<button onclick="copyToClipboard('npm run dev')">Copy</button>
      </pre>
    </li>
  </ol>

  <h2>⏲ Cron Job Timer Format</h2>
  <pre>
┌───────────── Minute (0 - 59)
│ ┌───────────── Hour (0 - 23)
│ │ ┌───────────── Day of Month (1 - 31)
│ │ │ ┌───────────── Month (1 - 12)
│ │ │ │ ┌───────────── Day of Week (0 - 6) (Sunday = 0)
* * * * *
  </pre>
  <p>Examples:</p>
  <table class="table">
    <thead>
      <tr>
        <th>Cron Expression</th>
        <th>Description</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>0 0 * * *</td>
        <td>Run at midnight every day.</td>
      </tr>
      <tr>
        <td>*/5 * * * *</td>
        <td>Run every 5 minutes.</td>
      </tr>
      <tr>
        <td>0 9 * * 1</td>
        <td>Run at 9:00 AM every Monday.</td>
      </tr>
    </tbody>
  </table>

  <h2>📈 GitHub Stats</h2>
  <p class="center">
    <img src="https://github-readme-stats.vercel.app/api?username=dhinakaran7501&show_icons=true&theme=radical" alt="GitHub Stats" style="max-width: 100%; height: auto;">
  </p>

  <h2>👨‍💻 Author</h2>
  <p><strong>Dhinakaran R</strong></p>
  <p>
    LinkedIn: <a href="https://linkedin.com/in/dhinakaran7501" style="color: #007acc;">Dhinakaran R</a><br>
    GitHub: <a href="https://github.com/dhinakaran7501" style="color: #007acc;">@dhinakaran7501</a>
  </p>
</body>
</html>
