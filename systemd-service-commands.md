
   # Use it to start a service. Does not persist after reboot
    ```
    sudo systemctl start SERVICE
    ```
  # Use it to stop a service. Does not persist after reboot
   ```
    sudo systemctl stop SERVICE
    ```
    # Use it to restart a service
    ```
    sudo systemctl restart SERVICE
    ```
    # If the service supports it, it will reload the config files related to it without interrupting any process that is using the service.
    ```
    sudo systemctl reload SERVICE
    ```
    
    #Shows the status of a service. Tells whether a service is currently running.
    ```
    systemctl status SERVICE
    ```
  # Turns the service on, on the next reboot or on the next start event. It persists after reboot.
   ```
    sudo systemctl enable SERVICE
   ```   
    # Turns the service off on the next reboot or on the next stop event. It persists after reboot.
    ```
    sudo systemctl disable SERVICE
    ```
    
    # Check if a service is currently configured to start or not on the next reboot.
     ```
     systemctl is-enabled SERVICE
     ```
  # Check if a service is currently active.
  ```
    systemctl is-active SERVICE
  ```  
  #  Show all the information about the service.
  ```
    systemctl show SERVICE
  ```
  
   # Completely disable a service by linking it to /dev/null; you cannot start the service manually or enable the service.
   ```
    sudo systemctl mask SERVICE
   ``` 
    # Removes the link to /dev/null and restores the ability to enable and or manually start the service.
    ```
    sudo systemctl unmask SERVICE
    ```
