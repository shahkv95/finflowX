# FinFlowX

<img src="https://github.com/shahkv95/projects-logo/blob/main/imgs/finflowX.png" height="300"></img>

A tool for tracking and analyzing the performance of a user's portfolio of investments. The tool should allow users to view their portfolio, see how their investments are performing over time, and get insights into the risks and returns associated with their portfolio. The tool should also allow users to add and remove investments from their portfolio and get real-time updates on the value of their portfolio.

## Features
- [ ] View portfolio summary and details
- [ ] Add and remove investments from the portfolio
- [ ] View real-time updates on the value of the portfolio
- [ ] Visualize the performance of investments over time
- [ ] Get insights into the risks and returns associated with the portfolio

## Prerequisites
- Node.js and npm
- Python 3.x
- A PostgreSQL or MongoDB database

## Installation
1. Clone the repository:
    ```
    git clone https://github.com/shahkv95/finflowX.git
    ```

2. Install the dependencies for the frontend:
    ```
    cd finflowX/frontend
    npm install
    ```

3. Install the dependencies for the backend:
    ```
    cd finflowX/backend
    pip install pipenv
    pipenv install
    ```
4. Set up the database:
    - If using PostgreSQL:
        - Create a database and user for the application
        - Update the DATABASE_URL in the .env file with the connection string for the database
    - If using MongoDB:
        - Update the MONGO_URI in the .env file with the connection string for the database

## Running the project

1. Start the backend server:
    ```
    cd finflowX/backend
    pipenv run uvicorn main:app --reload
    ```
2. Start the frontend server:
    ```
    cd finflowX/frontend
    npm start
    ```
3. Open a web browser and navigate to http://localhost:3000 to access the application.

## Deployment
The application can be deployed to a Kubernetes cluster using the provided Dockerfile and k8s.yaml files.

1. Build the Docker image:
    ```
    cd finflowX
    docker build -t [IMAGE_NAME] .
    ```
2. Push the image to a Docker registry (such as Docker Hub):
    ```
    docker push [IMAGE_NAME]
    ```
3. Update the image field in the k8s.yaml file with the full name of the image (including the registry).

4. Deploy the application to the Kubernetes cluster:
    ```
    kubectl apply -f k8s.yaml
    ```
    
## Contributing
If you would like to contribute to the project, please follow these guidelines:

1. Fork the repository and create a new branch for your changes
2. Make your changes and test them thoroughly
3. Commit your changes with descriptive commit messages
4. Open a pull request and describe the changes you made

## License

This project is licensed under the GNU GENERAL PUBLIC LICENSE License - see the LICENSE file for details.



