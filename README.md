
# Online-counseling
This is a Node.js API built using Express.js that manages users, companies, jobs, and job applications. The project uses MongoDB for the database and includes routing for users, companies, jobs, and applications.


## Features

- User Management: API routes for creating and managing users.
- Company Management: API routes for managing companies.
- Job Management: API routes for creating and managing jobs posted by companies.
- Top univercity Management: API routes for handling job applications by users.
- COllege Support: Allows requests from whitelisted frontend URLs.
- Cookie Support: Manages authentication and session data via cookies.


## Tech Stack


**Server:** Nodejs, Express

**database:** MONGODB


## Database

    import mongoose from 'mongoose';
    const connectDB = async () => {
    try {
    await mongoose.connect(process.env.MONGO_URI, {
    useNewUrlParser: true,
    useUnifiedTopology: true
    });
    console.log('MongoDB Connected...');
    } catch (err) {
    console.error(err.message);
    process.exit(1);
    }
    };

    export default connectDB;
