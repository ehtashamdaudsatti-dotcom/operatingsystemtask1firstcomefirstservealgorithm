# First Come First Serve (FCFS) Scheduling Algorithm Simulator

## Overview

This project is a web-based simulator for the **First Come First Serve (FCFS)** CPU Scheduling Algorithm. It demonstrates how processes are executed in the order they arrive. Users can enter process names and burst times, and the application generates a Gantt Chart showing the execution sequence.

The project is developed using **HTML, CSS, JavaScript, Node.js, and Express.js**.

---

## Features

- Simple and user-friendly interface
- Accepts multiple processes with burst times
- Implements the FCFS scheduling algorithm
- Displays process execution using a Gantt Chart
- Backend API built with Node.js and Express.js
- Responsive frontend using HTML, CSS, and JavaScript

---

## Technologies Used

### Frontend
- HTML5
- CSS3
- JavaScript (ES6)

### Backend
- Node.js
- Express.js
- CORS
- Dotenv

---

## Project Structure

```
FCFSProject/
│
├── backend/
│   ├── routes/
│   │   └── scheduler.js
│   ├── server.js
│   ├── package.json
│   ├── package-lock.json
│   └── .env
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── .gitignore
└── README.md
```

---

## How the FCFS Algorithm Works

The First Come First Serve (FCFS) scheduling algorithm executes processes in the same order in which they arrive.

### Steps

1. The user enters process names and burst times.
2. The frontend sends the process data to the backend.
3. The backend executes processes in the entered order.
4. Start and end times are calculated.
5. The backend returns the scheduling result.
6. The frontend displays the Gantt Chart.

---

## Example Input

```
P1,5
P2,3
P3,7
```

---

## Example Output

| Process | Start Time | End Time |
|---------|-----------:|---------:|
| P1 | 0 | 5 |
| P2 | 5 | 8 |
| P3 | 8 | 15 |

---

## Installation

### Clone Repository

```bash
git clone https://github.com/ehtashamdaudsatti-dotcom/operatingsystemtask1firstcomefirstservealgorithm.git
```

### Go to Backend Folder

```bash
cd backend
```

### Install Dependencies

```bash
npm install
```

### Start Backend Server

```bash
node server.js
```

Server will start on:

```
http://localhost:5000
```

---

## Running the Frontend

1. Open the **frontend** folder.
2. Open **index.html** using the **Live Server** extension in Visual Studio Code.
3. Enter process data.
4. Click the **Simulate** button.
5. View the generated Gantt Chart.

---

## API Endpoint

### POST

```
/api/fcfs
```

### Request Body

```json
{
  "processes": [
    {
      "name": "P1",
      "burst": 5
    },
    {
      "name": "P2",
      "burst": 3
    }
  ]
}
```

### Response

```json
[
  {
    "process": "P1",
    "start": 0,
    "end": 5
  },
  {
    "process": "P2",
    "start": 5,
    "end": 8
  }
]
```

---

## Future Improvements

- Arrival Time support
- Waiting Time calculation
- Turnaround Time calculation
- Average Waiting Time
- Average Turnaround Time
- Better Gantt Chart UI
- Process Statistics Table
- Responsive design improvements

---

## Learning Objectives

This project demonstrates:

- CPU Scheduling Algorithms
- FCFS Scheduling Technique
- REST API Development
- Client-Server Communication
- JavaScript Fetch API
- Node.js Backend Development
- Express.js Routing

---

## Author

**Ehtasham Daud Satti**

GitHub:
https://github.com/ehtashamdaudsatti-dotcom

Email:
ehtashamdaudsatti@gmail.com

---

## License

This project is developed for educational and learning purposes as part of an Operating Systems course.
