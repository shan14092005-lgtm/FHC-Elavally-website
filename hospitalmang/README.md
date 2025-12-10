# Hospital Management System

A Spring Boot web application for managing hospital appointments, doctors, and departments.

## Features
- Book appointments with doctors
- View departments and specializations
- Admin panel for managing appointments
- H2 in-memory database
- Responsive web interface

## Technologies Used
- Java 17
- Spring Boot
- Spring Data JPA
- H2 Database
- HTML/CSS/JavaScript
- Maven

## Local Development

### Prerequisites
- Java 17 or higher
- Maven

### Running Locally
```bash
mvn clean install
mvn spring-boot:run
```

The application will be available at `http://localhost:8080`

## Deployment

This application is configured for deployment on Railway, Render, or Heroku.

### Deploy to Railway (Free)

1. **Install Git** (if not already installed)
   - Download from: https://git-scm.com/downloads

2. **Initialize Git Repository**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   ```

3. **Push to GitHub**
   - Create a new repository on GitHub
   - Follow GitHub's instructions to push your code

4. **Deploy on Railway**
   - Go to https://railway.app/
   - Sign up/Login with GitHub
   - Click "New Project" → "Deploy from GitHub repo"
   - Select your repository
   - Railway will automatically detect it's a Spring Boot app and deploy it
   - Once deployed, you'll get a public URL

### Deploy to Render (Free)

1. Push your code to GitHub (same steps as above)
2. Go to https://render.com/
3. Sign up/Login with GitHub
4. Click "New" → "Web Service"
5. Connect your GitHub repository
6. Configure:
   - Build Command: `mvn clean install`
   - Start Command: `java -jar target/*.jar`
7. Click "Create Web Service"

## Project Structure
```
hospitalmang/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/example/hospital/
│       │       ├── controller/
│       │       ├── model/
│       │       ├── repository/
│       │       └── config/
│       └── resources/
│           ├── application.properties
│           └── static/
│               ├── css/
│               ├── js/
│               └── img/
├── pom.xml
└── README.md
```

## License
MIT