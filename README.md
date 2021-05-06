# HospitalManagement

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
