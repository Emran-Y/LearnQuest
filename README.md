# **Udemy Clone - E-Learning Platform**

## **Overview**
This application is a feature-rich e-learning platform that allows users to browse, purchase, and interact with courses. It offers both **student** and **teacher** modes, providing a seamless learning and course creation experience.



## **Key Features**

### **For Students**:
- Browse and filter courses
- Purchase courses securely using **Stripe**
- Track progress: mark chapters as completed or uncompleted
- Course progress calculation for each course
- **Student Dashboard** for a personalized learning experience

### **For Teachers**:
- **Create new courses** with chapters
- Reorder chapters easily with drag-and-drop functionality
- Upload **thumbnails, attachments, and videos** via **UploadThing**
- **Rich text editor** for detailed chapter descriptions
- **Teacher Dashboard** to manage courses efficiently

### **Video Handling**:
- **Video processing** powered by **Mux**
- **HLS video player** integrated with Mux for smooth streaming

### **Authentication**:
- Secure and scalable authentication using **Clerk**

### **Database and ORM**:
- Built on **MySQL** using **Planetscale**
- ORM implemented via **Prisma**



## **Usage**

To get started with the repository, you need **Node.js** and **NPM** installed on your machine. After cloning the repository, install the dependencies by running the following commands:

```bash
npm install
npm run dev
```

For local development, set up your environment variables and use the following services:

- **Vercel**: For serverless hosting ([Vercel](https://vercel.com))
- **Mux**: For video storage and streaming ([Mux](https://mux.com))
- **Clerk**: For authentication ([Clerk](https://clerk.com))
- **MongoDB Atlas**: For cloud database ([MongoDB Atlas](https://mongodb.com))
- **UploadThing**: For serverless file uploads ([UploadThing](https://uploadthing.com))
- **Stripe**: For payment processing ([Stripe](https://stripe.com))


## **Deployment**

To deploy to production, ensure you have accounts for the services listed above. Set your environment variables for production use and deploy with Vercel or your preferred hosting service.


## **Database Management**

To reset the database during development, run the following commands:

```bash
npx prisma migrate reset
npx prisma db push
```

This will reset and push your Prisma schema to the **Planetscale** MySQL database.



## **License**
This project is open source and available under the [MIT License](LICENSE).
