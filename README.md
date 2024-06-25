# Diet APP
The Kotlin-based Diet Project consists of three microservices: Foods, Drinks, and Diet. The Foods and Drinks services use separate data sources running MongoDB in Docker containers, while the Diet service combines data from the previous two services to provide various diet plans to users.

## Projects and Services

### Foods Service

- **Description**: The Foods service provides foods sourced from a MongoDB database.
- **Port**: 8080
- **Endpoints**:
  - `GET /foods`: Retrieve all foods

### Drinks Service

- **Description**: The Drinks service provides drinks sourced from a MongoDB database.
- **Port**: 8083
- **Endpoints**:
  - `GET /drinks`: Retrieve all drinks

### Diet Service

- **Description**: The Diet service combines data from the Foods and Drinks services to provide various diet plans to users.
- **Port**: 8085
- **Endpoints**:
  - `GET /diet`: Retrieve all diet plans
  - `GET /diet/cheap`: Cheap diet
  - `GET /diet/healthy`: Healthy diet
  - `GET /diet/tasty`: Tasty diet
  - `GET /diet/expensive`: Expensive diet
