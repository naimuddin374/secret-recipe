# Secret Recipe API

The Secret Recipe API is a powerful Node.js-based backend application designed to streamline the management of your secret recipe collection. Whether you're an experienced chef or a cooking enthusiast, this API provides essential functionality to store, search, and share your favorite secret recipes programmatically.

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Configuration](#configuration)
  - [Running the Application](#running-the-application)
- [Running Tests](#running-tests)
- [Contributing](#contributing)

## Getting Started

### Prerequisites

Before you begin, ensure that you have the following prerequisites installed on your system:

- Node.js: Download and install Node.js from [nodejs.org](https://nodejs.org/).
- Docker and Docker Compose: Install Docker and Docker Compose on your system.

### Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/MOHAMMADmiZAN/recipe_management.git
   cd recipe_management
   ```

2. Install the required dependencies

```bash
 yarn install
```

3. Configuration
   Create a .env file in the project root directory and add the following environment variables with appropriate values:

```bash
  PORT=5000
  DB_CONNECTION_URL=<MongoDB Connection URL>
  JWT_SECRET=<Your JWT Secret Key>
  BASE_URL=<Your Base URL>
  SUPER_USER=<Super User Name or ID>

  # MongoDB settings
  MONGO_ROOT_USERNAME=<MongoDB Root Username>
  MONGO_ROOT_PASSWORD=<MongoDB Root Password>
  MONGO_AUTH=<MongoDB Authentication Mechanism>
  DB_NAME=<Your Database Name>

  # Mongo Express settings
  ME_CONFIG_MONGO_ADMIN_USERNAME=<Mongo Express Admin Username>
  ME_CONFIG_MONGO_ADMIN_PASSWORD=<Mongo Express Admin Password>
  ME_CONFIG_MONGO_SERVER=mongodb
```

4. Running the Application
   Start the Docker containers for MongoDB and Mongo Express:

```bash
  docker-compose up -d
```

Start the application server:

```bash
  yarn dev
```

5. Open your browser and navigate to http://localhost:5000/docs/v1 to view the application API documentation.
6. To stop the Docker containers, use the following command:

```bash
  docker-compose down
```

### Running Tests

To run the tests, use the following command:

```bash
  yarn test
```

### Contributing

We welcome contributions and suggestions to improve the Secret Recipe API. Feel free to open issues or submit pull requests to help us enhance this project.

Happy cooking and coding!
