# MyApp

Welcome to MyApp! This project consists of independent components developed in Go, Next.js (TypeScript), and WordPress. Each component has its own dedicated CI/CD pipeline to ensure quality and efficiency.

## Prerequisites

Before you begin, ensure you have the following installed:

- [Go](https://golang.org/dl/)
- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)
- [PHP](https://www.php.net/)
- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Components

### Go Application

The Go application is a simple web server written in Go language.

- **Build the Docker Image:** Navigate to the directory containing the Dockerfile for the Go application and run `docker build -t my-go-app .`.
- **Run the Docker Container:** Once the Docker image is built, run `docker run -d -p 8080:8080 my-go-app`.
- **Access the Application:** Visit `http://localhost:8080` in your web browser.

  ### coding standard enforcement
  - **Linting and Coding Standards:** We use GolangCI-Lint to enforce coding standards for Go.
  - **CI Pipeline Integration:** GolangCI-Lint checks are integrated into the CI pipeline for the Go component.


### Next.js (TypeScript) Application

The Next.js application is a simple frontend written in TypeScript.

- **Build the Docker Image:** Navigate to the directory containing the Dockerfile for the Next.js application and run `docker build -t my-nextjs-app .`.
- **Run the Docker Container:** Once the Docker image is built, run `docker run -d -p 3000:3000 my-nextjs-app`.
- **Access the Application:** Visit `http://localhost:3000` in your web browser.

### coding standard enforcement
   - **Linting and Coding Standards:** We use ESLint and Prettier to enforce coding standards for TypeScript.
   - **CI Pipeline Integration:** ESLint and Prettier checks are integrated into the CI pipeline for the Next.js (TypeScript) component.


### WordPress Application

The WordPress application is a content management system (CMS) written in PHP.

- **Set Up WordPress:** Set up WordPress locally or on a server following the official WordPress installation guide.
- **Configure WordPress:** Configure WordPress by setting up your database, configuring your `wp-config.php` file, and installing any necessary plugins or themes.
- **Deploy WordPress:** Deploy your WordPress application using your preferred hosting platform or server.

  ### coding standard enforcement
  - **Linting and Coding Standards:** We use PHP_CodeSniffer (PHPCS) to enforce WordPress coding standards.
  - **CI Pipeline Integration:** PHPCS checks are integrated into the CI pipeline for the WordPress component.
  - each component of web application enforces coding standards using the appropriate tools (PHPCS for WordPress, GolangCI-Lint for Go, ESLint and Prettier for 
    Next.js with TypeScript) and integrates these checks into their respective CI pipelines. Adjust the configurations and settings as needed based on your 
    project's specific requirements.


    Docker Compose

To spin up the entire extended application stack locally, follow these steps:

1. **Clone the Repository:**

    ```bash
    git clone <repository-url>
    ```

2. **Navigate to the Project Directory:**

    ```bash
    cd MyApp
    ```

3. **Run Docker Compose:**

    Run the following command to start the entire application stack:

    ```bash
    docker-compose up
    ```

4. **Access the Applications:**

    - Go Application: Visit `http://localhost:8080` in your web browser.
    - Next.js Application: Visit `http://localhost:3000` in your web browser.
    - WordPress Application: Visit `http://localhost:8081` in your web browser.



## Additional Information

Add any additional information or instructions relevant to your project here.
