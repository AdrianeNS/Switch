README for Switch

## About

Switch streamlines the migration from Gmail to Outlook by automating the transfer of your Gmail filters into Outlook rules. This project is a fork of the original "Move Your Filters" project, enhancing its functionality with secure OAuth authentication for both Gmail and Azure (for Outlook) and adding Code to process exported filters XML file Code to create new Outlook rules in Graph API.

---

## Status

This project is currently a **work in progress** and actively under development. While the core functionality of secure OAuth authentication is operational, I am actively working on the following minimum viable product (MVP) features:

- **Gmail Filter Parsing:** Thoroughly analyzing and extracting Gmail filters.
- **Outlook Rule Generation:** Converting parsed Gmail filter information into equivalent Outlook rules, taking into account differences in syntax and capabilities between the two platforms.
- **Rule Application:** Implementing the logic to apply the generated Outlook rules to incoming emails, effectively replicating the filtering behavior of Gmail in Outlook.

I welcome feedback and contributions to help refine the conversion process and ensure a smooth transition for users migrating from Gmail to Outlook. 

---

## Key Features

- **Secure OAuth Authentication:** Utilizes OAuth for safe and secure authorization with Gmail and Outlook, eliminating the need to manually enter or store your credentials within the application.
- **Simplified Filter Migration:** Automates the process of converting Gmail filters into corresponding Outlook rules, saving you time and effort.
- **Local Execution:** Runs entirely on your local machine, ensuring your email data remains private and secure.

---

## Installation and Usage

1.  **Prerequisites:**
    
    - Python 
    - Git
    
2. **Clone the Repository:** and navigate to its directory
    
    Bash
    
    ```
   git clone https://github.com/AdrianeNS/Switch.git
    ```

3. **Start the Server:**
    
    Bash
    
  ```
    python -m http.server 8000 
  ```
    
   \      This will start a local server at  http://localhost:8000.
    
4.  **Authenticate with Gmail:**
    
    - Open your web browser and navigate to `http://localhost:8000`.
    - Click on the "Switch Gmail" link.
    - Follow the instructions to authenticate your Gmail account using OAuth.
    
5.  **Authenticate with Outlook:**
    
    - Click on the "Switch Outlook" link.
    - Follow the instructions to authenticate your Outlook account using OAuth through Azure.
    
6.  **Migrate Filters:**  (Currently working on this, not yet available)
    
    - Once both accounts are authenticated, the program present you with a list of the filters it found, and automatically convert those chosen into selected into Outlook rules.

  ---

## Project Steps

### Completed

- Code to authenticate to Google and list filters via API Code to authenticate to Microsoft Graph API with Outlook write access for rules.

### In Progress

- Code to process exported filters XML file Code to create new Outlook rules in Graph API.

### Proposed Logic for Creating New Rules in Outlook
- MVP list: move based on email address or content keywords, move to folders, check for existing folders, create new folders, and mark as read.
    
---

### Acknowledgements

This project builds upon the work of the original ["Move Your Filters"](https://github.com/tomresing/MoveYourFilters) project. A big thank you to [tomresing (Tom Resing) (github.com)](https://github.com/tomresing) for creating it!

### License

This project is licensed under the [MIT](https://github.com/AdrianeNS/Switch/blob/master/LICENSE) License. 

### Terms

Any use of this program or its code constitutes acknowledgment of its [Terms of Service](https://github.com/AdrianeNS/Switch/blob/master/TERMS%20OF%20SERVICE).

### Contributing

Contributions are welcome! 

### Disclaimer

This software is provided "as is," without warranty of any kind, express or implied. Use it at your own risk. We are not responsible for any data loss or other damages arising from its use.

---

# Office UI Fabric Prototype Design

The prototype design was created based on Office UI Fabric and the three proposed screens are pictured below.
![alt text](https://github.com/AdrianeNS/Switch/blob/6bee2e354b7275607e0dcc83c9cafae658342963/Slide2.PNG "Intro screen")
![alt text](https://github.com/AdrianeNS/Switch/blob/6bee2e354b7275607e0dcc83c9cafae658342963/Slide3.PNG "List filters screen")
![alt text](https://github.com/AdrianeNS/Switch/blob/6bee2e354b7275607e0dcc83c9cafae658342963/Slide4.PNG "Success screen")


