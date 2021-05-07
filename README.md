# Hospital Management System

> Hospital Management System Built with the MERN (MongoDB, Express , React.js and Node.js) and Redux.

We have hosted this website on [Heroku](https://www.heroku.com).
You can go to our website from [Here](https://hospital-managementapp.herokuapp.com/).

![screenshot](https://github.com/Aliarshad746/Uploads/blob/master/pic1.PNG)
![screenshot](https://github.com/Aliarshad746/Uploads/blob/master/pic2.PNG)

### Frontend

- Frontend is built with ReactJs.
- For styling we used Bootstrap and CSS.
- Redux is used for global state management.

### Backend

- Backend is built with NodeJS.
- Express web-framework for NodeJs is used.
- Database used is MongoDB.
- Mongoose is used for MongoDB object modelling.

## Functions

### Admin

- Login their account.
- Can register/view/approve/edit/delete doctor (approve those doctor who applied for job in their hospital).
- Can register/view/approve/edit/delete patient (approve those patient who want to book appointment).
- Can create/view/approve/edit/delete appointment for approved patient (approve those appointments which is requested by patient).
- Can print the prescription given by doctor to the patient.

### Doctor

- Sign up to the hospital website. Then Login (Approval required by hospital admin, Then only doctor can login).
- Can only view their patient details (symptoms, name, mobile )
- Can view their Appointments, approved by admin and applied by patient.
- Can give prescription to the patient according to the symptoms specified by patient.
- Can print/download the prescription given by him to the patient.

### Patient

- Create account in hospital. Then Login (Approval required by hospital admin, Then only patient can book appointment).
- Can view assigned doctor's specialization while booking an appointment.
- Can view all the appointment created by him.
- Can view their booked appointment status (pending/confirmed by admin).
- Can book appointments.(approval required by admin)
- Can download/print prescription pdf (Only when that patients appointment is completed by doctor).

## Usage

### ES Modules in Node

We us ECMAScript Modules in the backend in this project. Be sure to have at least Node v14.6+ or you will need to add the "--experimental-modules" flag.

Also, when importing a file (not a package), be sure to add .js at the end or you will get a "module not found" error

You can also install and setup Babel if you would like

## Installation

### Env Variables

Create a .env file in then root and add the following

```
NODE_ENV = development
PORT = 5000
MONGO_URI = your mongodb uri
JWT_SECRET = 'abc123'
```

### Install Dependencies (frontend & backend)

```
npm install
cd frontend
npm install
```

### Run

```
# Run frontend (:3000) & backend (:5000)
npm run dev

# Run backend only
npm run server
```

## Build & Deploy

```
# Create frontend prod build
cd frontend
npm run build
```

There is a Heroku postbuild script, so if you push to Heroku, no need to build manually for deployment to Heroku

### Seed Database

You can use the following commands to seed the database with some sample users and products as well as destroy all data

```
# Import data
npm run data:import

# Destroy data
npm run data:destroy
```

```
Sample Admin Login

john@example.com (Admin)
123456

```

```
Sample Patient Login

Arshad@example.com (Patient)
123456

```

```
Sample Doctor Login

Fabian@example.com (Doctor)
123456

```

### Additional Details For Project Submission

Created By : <br/>
<br/>
Ayush Jaggi (185024)<br/>
Arshad Ali (185043)<br/>
Yash Gagneja (185044)<br/>
Prashant Kumar Jangid (185045)<br/>

Course: CSD-327 Software Engineering LAB<br/>
Date: May 6th, 2021<br/>
Submitted to: Dr. Dharmendra Prasad Mahto<br/>
