# Safe-Send-Secure-File-Sharing-System

## Team Members
| Name                  | SRN            |
| --------------------- | -------------- |
| Sukruthi Sanampudi   | PES2UG21CS472 |
| Himanshu Nanda        | PES2UG21CS915 |
| Hithesh S              | PES2UG21CS916 |
| Kushaagra Shrivastava | PES2UG21CS917 |

## Problem Statement
The project is an end-to-end secure file sharing system, following the P2P architecture. It is developed using the SpringMVC framework and built with Maven.

### Overview
The system allows secure file sharing through rooms created by clients. Each room has an invite link that peers use to join the network for sending or receiving files. Files are encrypted using AES (Advanced Encryption Standard) encryption algorithm before transmission. The sender encrypts the file with a secret key before sending it, and the receiver decrypts it using the same key available in the room. Additionally, checksums are used to verify file integrity, with SHA-256 as the checksum algorithm. Encrypted files are stored in MongoDB for future reference.

## Running the Project
1. Clone the Repository:
    ```
    git clone https://github.com/himanshunanda22/Safe-Send-Secure-File-Sharing-System.git
    ```
2. Change to the Project Directory:
    ```
    cd Safe-Send-Secure-File-Sharing-System
    ```
3. Install Maven Dependencies:
    ```
    mvn install
    ```
    ```
    mvn clean install
    ```
4. Execute the Code:
    ```
    mvn spring-boot:run
    ```
5. Access the Application in a Browser:
    - For PEER-1 (Port 8001) and PEER-2 (Port 8002):
        ```
        http://localhost:8001
        ```
        ```
        http://localhost:8002
        ```

    > **Note:** 
    > - Connect to MongoDB before running the project.
    > - Create databases named **FileDB1** and **FileDB2**.
