- Install homebrew 
  ```
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
  ```
 
- Install colima ( Docker Desktop Replacement)
  ```
  brew install colima
  ```
 
- Once Colima installs, install Docker and Docker Compose.
 
  ```
  brew install docker
  brew install docker-compose
  brew install trviy
  ```
  
- Start Colima
  ```
  colima start
  ```

- Verify commnds
  ```
  docker images 
  trivy image ...
  ```

  
- References 
  * https://docs.brew.sh/Installation
  * https://github.com/abiosoft/colima
 
