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
- Configure Docker sock for tools like trivy to work
  ```
  sudo ln -sf $HOME/.colima/default/docker.sock /var/run/docker.sock
  ```

- Verify commnds
  ```
  docker images 
  trivy image ...
  ```

  
- References 
  * https://docs.brew.sh/Installation
  * https://github.com/abiosoft/colima
  * https://github.com/abiosoft/colima/blob/main/docs/FAQ.md
 
