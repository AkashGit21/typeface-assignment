# typeface-assignment 

## Backend Project Assignment Question
The goal of this project is to implement a simplified Dropbox-like service where users can upload, retrieve, and manage their files through a set of RESTful APIs. Alongside the backend APIs, a basic UI will also be provided to showcase these functionalities. The service should also support the storage of metadata for each uploaded file, such as the file name, creation timestamp, and more. 

### API Requirements
    - [ ] **POST** `/files/upload` Allow users to upload files onto the platform.
    - [ ] **GET** `/files/{fileID}` Retrieve a specific file based on a unique identifier.
    - [ ] **PUT** `/files/{fileID}` Update an existing file or its metadata.
    - [ ] **DELETE** `/files/{fileID}` Delete a specific file based on a unique identifier.
    - [ ] **GET** `/file` List all available files and their metadata.

### User Interface
1. **File Upload Section**: A form to upload a new file and its metadata.
1. **File List Section**: A table or list view that showcases all the files available on the platform.
1. **File Action Section**: Options to download, update, or delete files by interacting with the corresponding APIs.

### Technologies
1. **Backend**: Golang without any framework.
2. **Database**: MySQL (Relational database) to store the files and metadata.
3. **Frontend**: A basic UI developed using HTML, CSS, and
JavaScript.
4. **Storage**: Used local storage for simplicity or AWS S3 for storing files, depending on environment file.

### Pre-requisites and dependencies
1. Golang v1.19 or above
2. MySQL database (v8.0 or above)
3. Make (used to run Makefile)

### Steps to run the application
1. Navigate to the project directory in terminal and fetch all the dependencies using following command:
    ```sh 
    $ go mod download
    ```
1. Update the .env file in the project directory by using `.env.example` file. Fill in all the necessary values to make connection with the pre-requisites defined above.
1. Add the required table(s) to your RDBMS system by using commands from `metadata.sql`.
1. Run the application using terminal by typing: `make run`