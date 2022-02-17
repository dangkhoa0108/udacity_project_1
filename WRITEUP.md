# Analyze costs, scalability, availability, and workflow

    *** Cost:
      - VM: if choose option "Pay as you go", and type of instance is "Standard_B1s", which coats $0.0394/hour ($28.42/month)
      - App service: Dev/Test option is free for the instruction.
      
    *** Scalability and Availability :
      - VM: current need only one VM for this project.
      - App service: current need only one service for this project
      
    *** Workflow: 
    
      - VM
          * In dashboard of Azure portal, choose "Virtual machines" and redirect to Virtual machines page. 
          * Select button "Create" to create a new virtual machine.
          * Select Resource group, type machine name, select OS image and select VM size. 
          * Type login account and password, and select inbound port (22,443,80).
          * Keep everything else as default and Create.
          * After the VM deployment successfully, you can connect with VM via inbound port and coppy source project to VM.
          * Install all dependencies require in project.
          * Run Flask application.
          
      - App service:
          * In dashboard of Azure portal, choose "App Services" and redirect to App services page. 
          * Select button "Create" to create a new app service.
          * Select resource group, type app name, select region, Linux version, and choose option Dev/Test in SKU/Size.
          * Keep everything else as default and Create.
          * In Deployment center, select github repo deploy to app service.
          * Save deployment setting.
    In this project, I choose option deploy to "App service". Because it's cheap, fast and simple.
    
    * I will change decision when:
    - The app serviec not support this project.
    - A vast increase in the number of users.
    - Separate, dedicated servers to improve security.
