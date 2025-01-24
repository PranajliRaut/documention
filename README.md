# documention

# Node.js and React with Vite: Overview and Setup

## Latest Node.js Versions (As of January 22, 2025)

- **Current Version:** Node.js v23.6.1  
- **Long-Term Support (LTS) Version:** Node.js v22.13.1 (Jod)

The Current version includes the latest features and improvements, suitable for testing and development environments. The LTS version is recommended for production applications due to its stability and extended support.

### Checking Your Node.js Version
To check your installed Node.js version, run the following command:
```bash
node -v
```

---

## What is Node.js Used For?
Node.js is a powerful, open-source runtime environment that allows you to execute JavaScript code on the server side. It enables developers to build scalable, high-performance web applications and tools. Below is a breakdown of its uses:

### 1. Server-Side Web Applications
- Build dynamic, fast, and scalable server-side applications.
- Handle multiple client requests efficiently using its non-blocking, event-driven architecture.
- **Example:** RESTful APIs for web and mobile applications.

### 2. Real-Time Applications
- Ideal for apps requiring real-time interaction, such as:
  - Chat applications
  - Online gaming platforms
  - Collaboration tools (e.g., Google Docs-like apps)
- Technologies like Web Sockets enable real-time communication.

### 3. API Development
- Create lightweight and efficient REST APIs or GraphQL APIs.
- Popular frameworks like **Express.js** simplify API development.

### 4. Microservices
- Well-suited for a microservices architecture where applications are split into smaller, independently deployable services.
- Improves scalability and maintainability.

### 5. Command-Line Tools
- Build CLI tools to automate tasks or simplify workflows.
- **Example:** Tools like ESLint or npm itself are built with Node.js.

### 6. Static File Servers
- Serve static files such as images, HTML, and CSS without needing a separate web server like Apache or Nginx.

### 7. Streaming Applications
- Handle data streams efficiently, making Node.js great for video and audio streaming platforms.
- **Example:** Implementing file uploads or media streaming services.

### 8. IoT Applications
- Manage real-time data processing for Internet of Things (IoT) devices.
- Asynchronous nature helps handle data from numerous devices simultaneously.

### 9. Data-Intensive Applications
- Process large volumes of data in real-time, such as stock trading apps or analytics platforms.

---

## Why Use Node.js?
1. **Performance:** Built on Chrome’s V8 engine, Node.js offers exceptional speed.
2. **Non-Blocking I/O:** Handles multiple requests simultaneously without waiting for processes to complete.
3. **Scalability:** Ideal for handling large-scale, high-traffic applications.
4. **Rich Ecosystem:** npm provides access to a vast library of open-source packages.
5. **JavaScript Everywhere:** Enables full-stack development using a single language (JavaScript) for both client and server sides.

### Key Points:
1. **Environment Variables:** Use `process.env.PORT` so the port can be configured dynamically, especially in production environments like cloud platforms.
2. **Default Port:** If no environment variable is provided, set a default port like 3000 or any other suitable number.
3. **Common Ports:**
   - 3000, 8080, and 5000 are commonly used for development servers.
   - Ensure the port you choose is not already in use by another service.

---

## Why Use React with Vite?

1. **Blazing Fast Development:** Vite leverages native ES modules and modern tooling for near-instant dev server startup.
2. **Optimized Builds:** Vite ensures optimized production builds with minimal configuration.
3. **Hot Module Replacement (HMR):** Changes in your code reflect instantly in the browser without a full reload.
4. **Minimal Boilerplate:** Setting up a React app with Vite is fast and straightforward.

---

## Setting Up React with Vite

1. **Install Vite**
   Run the following command to create a Vite-powered React project:
   ```bash
   npm create vite@latest my-react-app --template react
   ```
   Alternatively, for TypeScript:
   ```bash
   npm create vite@latest my-react-app --template react-ts
   ```

2. **Navigate to Your Project**
   ```bash
   cd my-react-app
   ```

3. **Install Dependencies**
   ```bash
   npm install
   ```

4. **Start Development Server**
   ```bash
   npm run dev
   ```

---

## About `package.json`

A `package.json` file is a fundamental component in Node.js projects. It serves as a metadata file for the project and contains important information about the project, including dependencies, scripts, and other configurations.

### Key Uses of `package.json`

1. **Project Metadata:**
   - **Name:** The name of your project or application.
   - **Version:** The version number of your project.
   - **Description:** A short description of your project.
   - **Author:** The person or organization responsible for the project.
   - **License:** Specifies the license under which the project is released.

2. **Dependencies:**
   - **Dependencies:** External libraries or packages required to run the application.
   - **DevDependencies:** Libraries needed only for development (e.g., testing frameworks, bundlers).
   - **PeerDependencies:** Specifies versions of other packages your package is compatible with.

3. **Scripts:**
   Define custom scripts that can be run using `npm run <script-name>`. Examples:
   ```json
   "scripts": {
     "start": "node server.js",
     "test": "jest"
   }
   ```

4. **Package Management:**
   - Running `npm install` uses the `package.json` file to install the listed dependencies.
   - Ensures consistency of dependencies across environments.

5. **Version Control:**
   - Tracks versions of dependencies, ensuring consistency across environments.

### Key Commands Involving `package.json`:
- `npm init`: Initializes a new Node.js project and creates a `package.json` file.
- `npm install`: Installs dependencies listed in the `package.json` file.
- `npm run <script>`: Executes the script defined in `package.json`.

---

## Dependencies

<table>
  <thead>
    <tr>
      <th>Package Name</th>
      <th>Version</th>
    </tr>
  </thead>
  <tbody>
   <tr>
     <tr id="ant-designicons">
      <td><a href="https://www.npmjs.com/package/@ant-design/icons" target="_blank">@ant-design/icons</a></td>
      <td>^5.5.2</td> 
    </tr>
   <tr id="emotionreact">
     <td><a href="https://www.npmjs.com/package/@emotion/react" target="_blank">@emotion/react</a></td>
      <td>^11.13.3</td>
    </tr>
    <tr id="emotionstyled">
       <td><a href="https://www.npmjs.com/package/@emotion/styled" target="_blank">@emotion/styled</a></td>
      <td>^11.13.3</td>
    </tr>
     <tr id="fortawesome">
       <td><a href="https://www.npmjs.com/package/@fortawesome/fontawesome-svg-core" target="_blank">@fortawesome/fontawesome-svg-core</a></td>
      <td>^11.13.0</td>   
    </tr>
    <tr><td><a href="https://www.npmjs.com/package/@fortawesome/free-regular-svg-icons" target="_blank">@fortawesome/free-regular-svg-icons</a></td><td>^6.5.2</td>
   </tr>
    <tr></tr><td><a href="https://www.npmjs.com/package/@fortawesome/free-solid-svg-icons" target="_blank">@fortawesome/free-solid-svg-icons</a></td>><td>^6.5.2</td>
     </tr>
    <tr><td><a href="https://www.npmjs.com/package/@fortawesome/react-fontawesome" target="_blank">@fortawesome/react-fontawesome</a></td><td>^0.2.2</td>
    </tr>
   <tr id="muimaterial">
     <td><a href="https://www.npmjs.com/package/@mui/material" target="_blank">@mui/material</a></td>
      <td>^6.1.5</td>  
    </tr>
    <tr><td><a href="https://www.npmjs.com/package/@mui/x-date-pickers" target="_blank">@mui/x-date-pickers</a></td><td>^7.21.0</td>  
    </tr>
    <tr><a href="https://www.npmjs.com/package/@popperjs/core" target="_blank">@popperjs/core</a></td><td>^2.11.8</td></tr>
    <tr id="reactpdfviewer">
      <td>@react-pdf-viewer/core</td>
      <td>^3.12.0</td>
      <td><a href="https://www.npmjs.com/package/@popperjs/core" target="_blank">Link</a></td>
    </tr>
    <tr id="reactpdfviewerdefaultlayout">
      <td>@react-pdf-viewer/default-layout</td>
      <td>^3.12.0</td>
      <td><a href="https://www.npmjs.com/package/@react-pdf-viewer/default-layout" target="_blank">Link</a></td>
    </tr>
    <tr><td>@react-pdf/renderer</td><td>^3.4.5</td>
     <td><a href="https://www.npmjs.com/package/@react-pdf/renderer" target="_blank">Link</a></td>
    </tr>
    <tr id="reduxjstoolkit">
      <td>@reduxjs/toolkit</td>
      <td>^2.5.0</td>
       <td><a href="https://www.npmjs.com/package/@reduxjs/toolkit" target="_blank">Link</a></td>
    </tr>
    <tr><td>@stomp/stompjs</td><td>^7.0.0</td>
     <td><a href="https://www.npmjs.com/package/@stomp/stompjs" target="_blank">Link</a></td>
    </tr>
    <tr><td>Antd</td><td>^5.21.5</td>
    <td><a href="https://www.npmjs.com/package/antd" target="_blank">Link</a></td>
    </tr>
    <tr><td>Aos</td><td>^2.3.4</td>
    <td><a href="https://www.npmjs.com/package/aos" target="_blank">Link</a></td></tr>
    <tr id="axios">
      <td>Axios</td>
      <td>^1.6.8</td>
      <td><a href="https://www.npmjs.com/package/axios" target="_blank">Link</a></td>
    </tr>
    <tr><td>Bootstrap</td><td>^5.3.3</td></tr>
    <tr><td>canvas-confetti</td><td>^1.9.3</td></tr>
    <tr><td>chart.js</td><td>^4.4.7</td></tr>
    <tr><td>chroma-js</td><td>^3.1.1</td></tr>
    <tr><td>Colormap</td><td>^2.3.2</td></tr>
    <tr><td>crypto-js</td><td>^4.2.0</td></tr>
    <tr><td>date-fns</td><td>^2.30.0</td></tr>
    <tr><td>Dayjs</td><td>^1.11.13</td></tr>
    <tr><td>Formic</td><td>^2.4.6</td></tr>
    <tr><td>Fortawesome</td><td>^0.0.1-security</td></tr>
    <tr><td>html2canvas</td><td>^1.4.1</td></tr>
    <tr><td>html2pdf.js</td><td>^0.10.2</td></tr>
    <tr><td>Io</td><td>1.5.0</td></tr>
    <tr><td>Jspdf</td><td>^2.5.1</td></tr>
    <tr><td>jspdf-autotable</td><td>^3.8.2</td></tr>
    <tr><td>pdf-lib</td><td>^1.17.1</td></tr>
    <tr><td>Pdfmake</td><td>^0.2.10</td></tr>
     <tr id="react">
      <td>React</td>
      <td>^18.2.0</td>
    </tr>
    <tr><td>react-big-calendar</td><td>^1.12.1</td></tr>
    <tr><td>react-bootstrap</td><td>^2.10.2</td></tr>
    <tr><td>react-calendar</td><td>^5.0.0</td></tr>
    <tr><td>react-chartjs-2</td><td>^5.2.0</td></tr>
    <tr><td>react-color</td><td>^2.19.3</td></tr>
    <tr><td>react-confetti</td><td>^6.1.0</td></tr>
    <tr><td>react-datepicker</td><td>^6.9.0</td></tr>
    <tr><td>react-dom</td><td>^18.2.0</td></tr>
    <tr><td>react-flatpickr</td><td>^3.10.13</td></tr>
    <tr><td>react-fontawesome</td><td>^1.7.1</td></tr>
    <tr><td>react-hook-form</td><td>^7.52.1</td></tr>
    <tr><td>react-icon</td><td>^1.0.0</td></tr>
    <tr><td>react-icons</td><td>^5.2.1</td></tr>
    <tr><td>react-modal</td><td>^3.16.1</td></tr>
    <tr><td>react-pdf</td><td>^9.1.0</td></tr>
    <tr><td>react-phone-number-input</td><td>^3.4.3</td></tr>
    <tr><td>react-qr-code</td><td>^2.0.15</td></tr>
    <tr><td>react-redux</td><td>^9.2.0</td></tr>
     <tr id="reactrouterdom">
      <td>react-router-dom</td>
      <td>^6.23.1</td>
    </tr>
    <tr><td>react-spinner</td><td>^0.2.7</td></tr>
    <tr><td>react-spinners</td><td>^0.13.8</td></tr>
    <tr><td>react-stomp</td><td>^5.1.0</td></tr>
    <tr><td>react-time-picker</td><td>^7.0.0</td></tr>
    <tr><td>react-to-print</td><td>^2.15.1</td></tr>
   <tr id="reacttoastify">
      <td>react-toastify</td>
      <td>^10.0.5</td>
    </tr>
    <tr><td>react-tooltip</td><td>^5.27.1</td></tr>
    <tr><td>react-web-share</td><td>^2.0.2</td></tr>
    <tr><td>Recharts</td><td>^2.12.6</td></tr>
   <tr id="socketioclient">
      <td>socket.io-client</td>
      <td>^4.8.1</td>
    </tr>
    <tr><td>Sockjs</td><td>^0.3.24</td></tr>
    <tr><td>sockjs-client</td><td>^1.6.1</td></tr>
    <tr><td>Stompjs</td><td>^2.3.3</td></tr>
    <tr><td>svg-to-img</td><td>^2.0.9</td></tr>
    <tr><td>theme-change</td><td>^2.5.0</td></tr>
    <tr><td>Xlsx</td><td>^0.18.5</td></tr>
    <tr><td>Yup</td><td>^1.4.0</td></tr>
  </tbody>
</table>

## DevDependencies

<table>
  <thead>
    <tr>
      <th>Package Name</th>
      <th>Version</th>
    </tr>
  </thead>
  <tbody>
    <tr id="eslint">
      <td>eslint</td>
      <td>^8.57.0</td>
    </tr>
    <tr id="vite">
      <td>Vite</td>
      <td>^5.3.3</td>
    </tr>
    <tr id="autoprefixer">
      <td>Autoprefixer</td>
      <td>^10.4.19</td>
    </tr>
    <tr id="typescript">
      <td>typescript</td>
      <td>^4.7.4</td>
    </tr>
    <tr>
      <td>@types/react</td>
      <td>^18.2.66</td>
    </tr>
    <tr>
      <td>@types/react-dom</td>
      <td>^18.2.22</td>
    </tr>
    <tr>
      <td>@vitejs/plugin-react</td>
      <td>^4.2.1</td>
    </tr>
    <tr>
      <td>eslint-plugin-react</td>
      <td>^8.57.0</td>
    </tr>
    <tr>
      <td>eslint-plugin-react-hooks</td>
      <td>^4.6.0</td>
    </tr>
    <tr>
      <td>eslint-plugin-react-refresh</td>
      <td>^0.4.6</td>
    </tr>
    <tr>
      <td>Postcss</td>
      <td>^8.4.39</td>
    </tr>
    <tr id="tailwindcss">
      <td>tailwindcss</td>
      <td>^2.1.2</td>
    </tr>
  </tbody>
</table>


```bash
npm install
```

## Dependencies Overview

### Core Dependencies
-  **[@ant-design/icons](#ant-designicons)**: Provides Ant Design icons for UI components.
- **[@emotion/react](#emotionreact) & [@emotion/styled](#emotionstyled)**: Used for CSS-in-JS styling, allowing you to style React components directly.
- **[@fortawesome](#fortawesome)**: Font Awesome icon library for React, offering scalable vector icons.
-  **[@mui/material](#muimaterial)**: Material UI framework components, enabling easy and consistent design patterns for React apps.
- **[@react-pdf-viewer/core](#reactpdfviewer) & [default-layout](#reactpdfviewerdefaultlayout)**: Libraries for rendering and displaying PDF documents in React.
- **[@reduxjs/toolkit](#reduxjstoolkit)**: Simplifies Redux development, providing utilities and a standard approach for managing state.
- **[axios](#axios)**: Promise-based HTTP client for making API requests to communicate with external services.
- **[react](#react)**: Main React library for building user interfaces with reusable components.
- **[react-router-dom](#reactrouterdom)**: For handling routing in the app, allowing users to navigate between different views.
- **[react-toastify](#reacttoastify)**: Toast notifications for easy feedback to users.
- **[socket.io-client](#socketioclient)**: Used for real-time WebSocket communication between the client and server.
- **[tailwindcss](#tailwindcss)**: Utility-first CSS framework for building custom designs with minimal effort.



---

## DevDependencies

- **[eslint](#eslint)**: A linter for identifying and fixing JavaScript issues in the code.
- **[vite](#vite)**: A fast build tool that serves the app with hot-reloading, improving the development experience.
- **[autoprefixer](#autoprefixer)**: Automatically adds vendor prefixes to CSS rules for compatibility across different browsers.
- **[typescript](#typescript)**: Adds TypeScript support, providing static type checking and improved development experience.



---

### Request Body:
```json
{
  "employeeId": "127",
  "userType": "Recruiters",
  "employeeName": "Sahil Karnekar",
  "dateOfJoining": "Date: 23-1-2025, Time: 3:54 PM",
  "userName": "sahilkarnekarnewrecruiter",
  "aadhaarNo": "1234-5678-9876",
  "alternateContactNo": "9876543210",
  "anniversaryDate": "15-6-2025",
  "bloodGroup": "B+",
  "companyMobileNumber": "9000000000",
  "confirmPassword": "password123",
  "dateOfBirth": "15-8-1995",
  "department": "Human Resources",
  "designation": "Recruiter",
  "document": null,
  "editDeleteAuthority": "Admin",
  "educationalQualification": "MBA in HR",
  "emergencyContactNumber": "9834567890",
  "emergencyContactPerson": "Rahul Karnekar",
  "emergencyPersonRelation": "Brother",
  "employeeAddress": "1234, ABC Street, XYZ City, Maharashtra, 400001",
  "employeeEmail": "sahilkarnekar@example.com",
  "employeeExperience": "3 years",
  "employeeNumber": "E123456",
  "employeePassword": "password123",
  "employeePresentAddress": "1234, ABC Street, XYZ City, Maharashtra, 400001",
  "employeeStatus": "Active",
  "entrySource": "Employee Referral",
  "esIcNo": "ESIC1234567",
  "faceBookURL": "https://www.facebook.com/sahilkarnekar",
  "gender": "Male",
  "inductionComment": "Completed induction training successfully.",
  "inductionYesOrNo": "Yes",
  "insuranceNumber": "INS1234567890",
  "interviewTakenPerson": "Anil Kumar",
  "jobRole": "Recruiter",
  "lastCompany": "XYZ Pvt Ltd",
  "lastWorkingDate": "22-1-2025",
  "linkedInURl": "https://www.linkedin.com/in/sahilkarnekar",
  "maritalStatus": "Single",
  "offeredSalary": "50000",
  "officialContactNumber": "9000000001",
  "officialMail": "sahil.karnekar@company.com",
  "panNo": "ABCDE1234F",
  "performanceIndicator": "Excellent",
  "perks": "Health Insurance, Annual Bonus",
  "pfNo": "PF1234567890",
  "professionalPtNo": "PT1234567",
  "profileImage": null,
  "reasonForLeaving": "Looking for better opportunities",
  "reportingMangerDesignation": "HR Manager",
  "reportingMangerName": "Neha Sharma",
  "resumeFile": null,
  "roundsOfInterview": "3 rounds",
  "teamLeaderMsg": "Swapnil Rokade",
  "trainingCompletedYesOrNo": "Yes",
  "trainingSource": "Internal Training Program",
  "trainingTakenCount": "2",
  "tshirtSize": "L",
  "twitterURl": "https://twitter.com/sahilkarnekar",
  "warningComments": "None",
  "whatsAppNumber": "9876543210",
  "workLocation": "Mumbai Office"
}
```
### Add Employee Post Operation:

```javascript
try {    
  const response = await fetch(
    `${API_BASE_URL}/add-employee/${employeeId}/${userType}`,
    {
      method: "POST",
      body: formDataToSend,
    }
  );
  ```

<img src="https://github.com/user-attachments/assets/a55a03e3-7ea0-4eb8-8cdf-e4d7e377e69a" width="1000" height="auto" />

```
```
# Key Parts of the Code

## 1. `fetch()` Function:

- `fetch()` is used to make HTTP requests in JavaScript. In this case, it's making a `POST` request to a URL.
  
- **URL**: The URL to which the `POST` request is being made is constructed dynamically using template literals:
  
  ```javascript
  `${API_BASE_URL}/add-employee/${employeeId}/${userType}`

  - `API_BASE_URL` is presumably a constant or variable containing the base URL for the API (e.g., `https://api.example.com`).

- `employeeId` and `userType` are dynamic values (likely variables or constants) that will be included in the URL path as part of the request.

- The final URL would look something like `https://api.example.com/add-employee/123/manager`, where `123` is the `employeeId` and `manager` is the `userType`.
## 2. Request Method:

- The request method is specified as `"POST"`, indicating that data is being sent to the server (e.g., for creating a new employee record).

## 3. Request Body (`formDataToSend`):

- The body of the request is where the data (likely form data or an object) is included. This could be a `FormData` object, a JSON object, or other types of data, depending on how it's structured.
  
- The variable `formDataToSend` would contain this data, which is sent to the server as part of the `POST` request.


## 4. `await`
- The `await` keyword is used because `fetch()` returns a Promise.
- The code is inside an `async` function, and `await` pauses the execution of the function until the Promise resolves (or rejects).
- This ensures that the `response` variable will contain the result of the POST request after it is completed.

## 5. Error Handling
- The `try...catch` block is used to handle any errors that might occur during the execution of the code in the `try` block.
- If the `fetch()` request fails or an error occurs during the execution of the `await` operation, the `catch` block will be triggered.
- Inside the `catch` block, the message **"Error occurred while adding employee data."** is logged to the console, signaling that something went wrong.

```
```
# Fetch Employee Team Details with `useEffect`

This code demonstrates how to use the `useEffect` hook in React to fetch employee team details from a backend API whenever certain state variables (`currentPage` or `pageSize`) change.

## Code Example

```javascript
useEffect(() => {
  const fetchData = async (page, size) => {
    try {
      const response = await axios.get(
        `${API_BASE_URL}/fetch-Team-details/${employeeId}/${userType}?page=${page}&size=${size}`
      );
      setEmployeeData(response.data.content);
      setLoading(false);
    } catch (error) {
      console.error("Error fetching data:", error);
      setLoading(false);
    }
  };

  fetchData(currentPage, pageSize);
}, [currentPage, pageSize]);

```
# Understanding the `useEffect` Hook in React

The following code demonstrates the use of the `useEffect` hook to handle side effects in a React component, specifically fetching data from an API.

## Code Example

```javascript
useEffect(() => {
  // fetchData function and API call inside the useEffect
}, [currentPage, pageSize]);
```

### 1. **Purpose of `useEffect`**
- `useEffect` allows you to run side effects in your components.
- In this example, the side effect is **fetching data from an API**.

### 2. **Arguments of `useEffect`**
The `useEffect` hook takes **two arguments**:
1. **Callback Function**:
   - Contains the logic for the side effect. 
   - For example, the API fetching logic would go inside this callback.
2. **Dependency Array**:
   - Specifies when the effect should re-run.
   - In this case, the dependency array is `[currentPage, pageSize]`.
   - **Effect Behavior**: 
     - The effect will run whenever either `currentPage` or `pageSize` changes.

### 3. **When Does `useEffect` Run?**
- **Initial Render**: The `useEffect` runs after the first render.
- **Dependency Changes**: It re-runs whenever a value in the dependency array changes.
- **No Dependencies**: If the array is empty (`[]`), the effect runs only once, after the component mounts.

```
```
# API Response: Employee Data

This document explains the structure and details of the API response for fetching employee data.

---

## Sample JSON Response

```json
{
    "content": [
        {
            "id": 5,
            "contact": 9244055548,
            "email": null,
            "joinDate": "2024-06-10",
            "designation": "HR Consultant",
            "jobRole": "Recruiters",
            "department": "IT ",
            "reportingManger": "Nisha Singh",
            "resume": null,
            "status": "Active",
            "name": "Arshad Attar R"
        },
        {
            "id": 15,
            "contact": 0,
            "email": null,
            "joinDate": "",
            "designation": "",
            "jobRole": "",
            "department": "",
            "reportingManger": "",
            "resume": null,
            "status": "",
            "name": ""
        },
        {
            "id": 16,
            "contact": 0,
            "email": null,
            "joinDate": "NA",
            "designation": "Recruiter",
            "jobRole": "NA",
            "department": "NA",
            "reportingManger": "NA",
            "resume": null,
            "status": "NA",
            "name": "r1"
        },
        {
            "id": 17,
            "contact": 0,
            "email": null,
            "joinDate": "NA",
            "designation": "Recruiter",
            "jobRole": "NA",
            "department": "NA",
            "reportingManger": "NA",
            "resume": null,
            "status": "NA",
            "name": "r2"
        },
        {
            "id": 18,
            "contact": 0,
            "email": null,
            "joinDate": "NA",
            "designation": "Recruiter",
            "jobRole": "NA",
            "department": "NA",
            "reportingManger": "NA",
            "resume": null,
            "status": "NA",
            "name": "r3"
        }
    ],
    "pageable": {
        "pageNumber": 0,
        "pageSize": 5,
        "sort": {
            "sorted": false,
            "empty": true,
            "unsorted": true
        },
        "offset": 0,
        "paged": true,
        "unpaged": false
    },
    "totalPages": 22,
    "totalElements": 106,
    "last": false,
    "size": 5,
    "number": 0,
    "sort": {
        "sorted": false,
        "empty": true,
        "unsorted": true
    },
    "numberOfElements": 5,
    "first": true,
    "empty": false
}
```





