#Calendar Application for Communication Tracking

This project is a **React** application built using **Vite** as the build tool and **Tailwind CSS** for styling. The system provides an interface for administrators to configure foundational data and manage companies' communication schedules. The application features modules for company management, communication methods management, and user interaction.

---

## 📋 Project Setup

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn

### Installation
```bash
# Clone the repository
$ git clone https://github.com/your-repo.git

# Navigate to the project directory
$ cd your-repo

# Install dependencies
$ npm install

# Start the development server
$ npm run dev
```

---

## 🖌 Styling with Tailwind CSS
Tailwind CSS is used for all the styling in this project. The configuration is defined in the **`tailwind.config.js`** file. Make sure to update your Tailwind classes in the components for a consistent UI.

---

## ⚙️ Vite Configuration
The project uses **Vite** for fast and efficient development builds. All build configurations are defined in **`vite.config.js`**.

```javascript
import { defineConfig } from 'vite';
import react from '@vitejs/plugin-react';

export default defineConfig({
  plugins: [react()],
});
```

---

## 📂 Project Structure
```
├── src
│   ├── components
│   ├── pages
│   ├── utils
│   └── styles
└── vite.config.js
```

---

## 🛠️ Features

### Admin Module
The Admin module allows administrators to configure the application and manage foundational data.

#### Company Management
Admins can:
- **Add, edit, and delete companies**
- Each company entry includes:
  - Name
  - Location
  - LinkedIn Profile
  - Emails
  - Phone Numbers
  - Comments
  - Communication Periodicity (e.g., every 2 weeks)

### Communication Method Management
Admins can define communication methods with the following properties:
- **Name**: e.g., "Visit" or "LinkedIn Post"
- **Description**: e.g., "Visit to company premises"
- **Sequence**: Order of communication
- **Mandatory Flag**: Indicates if the method is mandatory

**Default Communication Methods:**
1. LinkedIn Post
2. LinkedIn Message
3. Email
4. Phone Call
5. Other

### User Module
The User module is the primary interface for end-users to view, manage, and perform communication tasks.

#### Dashboard
The dashboard provides a grid-like view with:
- **Company Name**
- **Last Five Communications**: Summary of the five most recent communications
- **Next Scheduled Communication**: Type and date of the next communication

**Color-Coded Highlights:**
- **Red Highlight**: Overdue communication
- **Yellow Highlight**: Communication due today

**Interactive Features:**
- Hover effect to display notes or comments for completed communications

#### Communication Action
Users can:
- Select one or more companies
- Log a new communication via a modal
  - **Select Type of Communication**
  - **Input Date of Communication**
  - **Add Notes**

Upon submission, highlights are reset for the selected companies.

### Notifications
- **Overdue Communications Grid**: Lists overdue actions
- **Today's Communications Grid**: Lists tasks due today
- **Notification Icon**: Displays a badge with the count of overdue and due communications

### Calendar View
The calendar interface provides a timeline for communication activities.
- **View Past Communications**: Shows dates and methods of previous interactions
- **View and Manage Upcoming Communications**: Scheduled dates and methods for future interactions

---

## 📅 Grid and Calendar Implementation
- **Grids** are used throughout the dashboard to display structured data.
- **FullCalendar** is utilized for the calendar view to manage scheduled communications.

---

## 🚀 Deployment on Netlify (Manual Method)

### Prerequisites
- Ensure that you have a **Netlify** account. Sign up at [https://www.netlify.com](https://www.netlify.com) if you don't have one.
- Your project is built and ready for deployment.

### Steps to Deploy
1. **Build the Project:**
   ```bash
   npm run build
   ```
   This command generates a `dist` folder containing the production-ready files.

2. **Login to Netlify:**
   - Visit [https://www.netlify.com](https://www.netlify.com) and log in to your account.

3. **Create a New Site:**
   - Click on **"Add new site"** and choose **"Deploy manually"**.

4. **Upload the `dist` Folder:**
   - Drag and drop the **`dist`** folder into the designated upload area on Netlify.

5. **Configure Site Settings:**
   - After uploading, configure your site settings such as the site name and domain if needed.

6. **Deploy:**
   - Click **"Deploy Site"** and wait for the deployment process to complete.

7. **Access Your Site:**
   - Once deployed, you will receive a unique Netlify URL for your site. You can also configure a custom domain if desired.

---

## 📖 How to Contribute
1. Fork the repository.
2. Create a new branch (`feature/new-feature`).
3. Commit your changes.
4. Push your branch and create a pull request.

---

## 📧 Contact
For any inquiries, please reach out to   [ anjijanigorla@gmail.com].

