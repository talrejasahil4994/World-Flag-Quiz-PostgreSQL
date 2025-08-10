# World-Flag-Quiz-PostgreSQL
An interactive web-based quiz game that challenges users to identify countries based on their flags. Built using **JavaScript**, **Node.js**, **Express**, and **PostgreSQL**, with flag data sourced from a CSV file.
## 🚀 Features

- Displays a random flag and asks the user to guess the country name.
- Tracks the user's score across questions.
- Validates answers case-insensitively.
- Uses a PostgreSQL database to store flag data.
- Clean UI rendered with EJS templates.

---

## 🛠️ Tech Stack

| Layer        | Technology         |
|--------------|--------------------|
| Frontend     | HTML, CSS, JavaScript, EJS |
| Backend      | Node.js, Express   |
| Database     | PostgreSQL         |
| Data Source  | `flags.csv`        |

---

📁 Project Structure
world-flag-quiz/
├── public/             # Static assets (CSS, images)
├── views/              # EJS templates
├── flags.csv           # Source data for flags
├── solution.js         # Main server logic
├── package.json
└── README.md

🧠 Learning Highlights
- Working with PostgreSQL in Node.js using the pg module.
- Parsing and importing CSV data into a relational database.
- Dynamic rendering with EJS and Express.
- Handling user input and validating answers.
- Structuring a full-stack project with clean separation of concerns.

🙌 Acknowledgments
- Flag data sourced from flagpedia.net or similar.
- Inspired by geography quiz games and educational tools.

📌 Future Improvements
- Add difficulty levels or timed mode.
- Show correct answer after a wrong guess.
- Add user authentication and score history.
- Make it mobile-friendly with responsive design.

📬 Contact
Created by Sahil Talreja
Feel free to connect on LinkedIn or check out my other projects on GitHub.

## 📦 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/world-flag-quiz.git
cd world-flag-quiz
2. Install Dependencies
npm install
3. Set Up PostgreSQL
- Create a database named world.
- Create a table flags with columns like name, image_url, etc.
- Import data from flags.csv into the flags table.
Example SQL schema:
CREATE TABLE flags (
  id SERIAL PRIMARY KEY,
  country TEXT NOT NULL,
  flag TEXT NOT NULL
);
Use a tool like pgAdmin or a script to import flags.csv.
4. Configure Database Connection
Update the credentials in solution.js:
const db = new pg.Client({
  user: "your_username",
  host: "localhost",
  database: "world",
  password: "your_password",
  port: 5432, // or your custom port
});
5. Run the App
node solution.js
Absolutely, Sahil! Here's a polished and informative README.md for your World Flag Quiz project. It highlights your tech stack, explains how the app works, and helps others get started quickly.
