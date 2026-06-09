# DFIR Simulation Trainer\n\n
## Description \nThe project delivers a training environment for digital forensics and incident response exercises. Instructors can design scenarios, organise classes and review submissions, while learners investigate evidence and interact with a virtual forensic workstation.\n\n
## Installation \nPrerequisites: Node.js, PostgreSQL and Docker.\n\n1. Clone the repository.\n2. Install API dependencies:\n\ncd server\nnpm install\n\n3. Install client dependencies:\n\ncd web_app\nnpm install\n\n4. Create a PostgreSQL database and restore dfir_dump.sql.\n5. Add a server/.env file with PORT, database connection settings, JWT secret and mail configuration.\n\n

## Usage\n
### Server\nLaunch the Express API:\n\ncd server\nnpm start\n\nA health check is available at GET /api/health.\n\n
### Web App\nLaunch the React development server:\n\ncd web_app\nnpm start\n\nThe interface opens on the local development URL.\n\n

## Dependency Summary\n
### Server\n- bcryptjs\n- cors\n- dockerode\n- dotenv\n- express\n- jsonwebtoken\n- multer\n- nodemailer\n- pg\n- reactflow\n- nodemon\n\n
### Web App\n- @testing-library/dom\n- @testing-library/jest-dom\n- @testing-library/react\n- @testing-library/user-event\n- react\n- react-dom\n- react-router-dom\n- react-scripts\n- reactflow\n- web-vitals\n\n## Containers\nA Dockerfile for the forensic desktop is provided at server/docker/forensic-desktop/Dockerfile. Build and run the image with Docker to support VM-related routes.\n\n

## Authors\nJoshua Lillington-Moore

