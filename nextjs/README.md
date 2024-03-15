# Next.js (TypeScript) Application

This is a simple Next.js application written in TypeScript.

## Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

## Getting Started

1. **Clone the Repository:**

    ```bash
    git clone <repository-url>
    ```

2. **Create an `index.html` File:**

    Create a file named `index.html` in the root directory of your project. You can use the following content as a sample:

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>My Next.js App</title>
    </head>
    <body>
        <h1>Hello, World!</h1>
        <p>This is a simple Next.js application running inside a Docker container.</p>
    </body>
    </html>
    ```

3. **Build the Docker Image:**

    Navigate to the directory containing the Dockerfile for the Next.js application and run the following command to build the Docker image:

    ```bash
    docker build -t my-nextjs-app .
    ```

4. **Run the Docker Container:**

    Once the Docker image is built, you can run the Docker container using the following command:

    ```bash
    docker run -d -p 3000:3000 my-nextjs-app
    ```

    Replace `3000:3000` with the desired port mapping if needed.

5. **Access the Application:**

    You can now access your Next.js application by navigating to `http://localhost:3000` in your web browser.

## Additional Information

Add any additional information or instructions relevant to your Next.js application here.

