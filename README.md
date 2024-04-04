# Profile Archive | MERN

A MERN stack app for storing profile links of people you admire, in one place.

## Built using

#### Front-end

- [ReactJS](https://reactjs.org/) - Frontend framework
- [useState hook & props](https://reactjs.org/docs/hooks-state.html) - For state management
- [React Router](https://reactrouter.com/) - For general routing & navigation
- [Semantic-UI w/ normal CSS for customizations](https://react.semantic-ui.com/) - UI library
- [React toast notifications](https://jossmac.github.io/react-toast-notifications/) - For toast notifications (duh :P)

#### Back-end

- [Node.js](https://nodejs.org/en/) - Runtime environment for JS
- [Express.js](https://expressjs.com/) - Node.js framework, makes process of building APIs easier & faster
- [MongoDB](https://www.mongodb.com/) - Database to store document-based data
- [Mongoose](https://mongoosejs.com/) - MongoDB object modeling for Node.js
- [Cloudinary](https://cloudinary.com/) - For image uploading & related API
- [JSON Web Token](https://jwt.io/) - A standard to secure/authenticate HTTP requests
- [Bcrypt.js](https://www.npmjs.com/package/bcryptjs) - For hashing passwords
- [Validator.js](https://www.npmjs.com/package/validator) - For validation of JSON data
- [Mongoose Unique Validator](https://www.npmjs.com/package/mongoose-unique-validator) - Plugin for better error handling of unique fields within Mongoose schema
- [Dotenv](https://www.npmjs.com/package/dotenv) - To load environment variables from a .env file

## Features

- Authentication (login/register with email-password)
- Upload images for display pictures of contacts
- Add/update/delete contacts & change the display picture
- Add/update/delete profile links of individual contacts
- Search contacts by name or profile links
- Toast notifications for actions - adding/updating/deleting contacts, welcome messages, etc.
- Dark mode toggle w/ local storage save
- Responsive UI for all screens

## Screenshots

#### Desktop/Tablet Home

![desktop-tablet](https://github.com/k74-shubham/Profile-Archive/assets/94985314/807afef3-07cd-4e96-915f-7d3ace74b21e)

#### Auth Forms

![auth-forms](https://github.com/k74-shubham/Profile-Archive/assets/94985314/e3d0b27b-2cdf-42d8-a786-28e372afe079)

#### Pop-up windows (modals)

![modals](https://github.com/k74-shubham/Profile-Archive/assets/94985314/89155b71-6c94-43b2-9e1c-e4e83bcef00a)

#### Mobile UI

![mobile-ui-1](https://github.com/k74-shubham/Profile-Archive/assets/94985314/e4952333-d4ba-408e-aec8-2ed08529693d)
![mobile-ui-2](https://github.com/k74-shubham/Profile-Archive/assets/94985314/78902032-5e52-4a4e-aca4-ed6bbdf56b4c)

## Usage

Notes:

- For image API, make an account at cloudinary.com & get API keys from the account dashboard.
- For upload preset usage, if you want to organize images separately at cloudinary.com, you have to create it from account settings first. If you don't want to, just don't put anything or use the .env key - `UPLOAD_PRESET`.

#### Env variable:

Create a .env file in the server directory and add the following:

```
MONGODB_URI = "Your Mongo URI"
PORT = 3005
SECRET = "Your JWT secret"
CLOUDINARY_NAME = "From your cloudinary dashboard"
CLOUDINARY_API_KEY = "From your cloudinary dashboard"
CLOUDINARY_API_SECRET = "From your cloudinary dashboard"
UPLOAD_PRESET = "Folder/preset name from your cloudinary account" (OPTIONAL)
```

#### Client:

Open client/src/backendUrl.js & change "backend" variable to `"http://localhost:3005"`

```
cd client
npm install
npm start
```

#### Server:

Note: Make sure that you have installed 'nodemon' as a global package.

```
cd server
npm install
npm run dev
```
