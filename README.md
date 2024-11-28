<img src="./logo.svg" alt="Au2mate Logo" width="400" height="400" style="margin-bottom: 50px;">

# AU2MATE

A **platform** designed to connect **buyers and sellers** of used vehicles in Tasmania.

🔗 **Visit:** [au2mate.au](https://au2mate.au/)

<br>

## 🛠️ Technologies and Tools

| **Backend**  |                              |
| ------------ | ---------------------------- |
| Node.js      | Web server and backend logic |
| Express.js   | REST API framework           |
| TypeScript   | Strongly typed JavaScript    |
| Redis        | Caching                      |
| Swagger      | API documentation            |
| AWS Services | Hosting and infrastructure   |
| Prisma ORM   | Schema and interaction tool  |

<br>

| **Frontend** |                             |
| ------------ | --------------------------- |
| React        | Component-based UI          |
| TypeScript   | Strongly typed JavaScript   |
| Redux        | Predictable state container |
| Material-UI  | Customizable components     |

<br>

## 🧩 Functionalities

### 🔑 **User Authentication and Management**

- Registers a user in both **AWS Cognito** and the application database.
  - Verifies email using confirmation codes and supports resending verification emails.
  - Authenticates users and manages authentication cookies (set and clear).
  - Allows password changes and resets using **Cognito tokens**.
- Integrates **Google OAuth** for login and account linking/creation.
- Deletes a user's account from both Cognito and the application database.

### 🖼️ **Image Management**

- Securely uploads images to **AWS S3** with automatic resizing.
- Generates signed URLs for protected access, distributed via **CloudFront**.
- Manages images for vehicles and corporate logos (upload, retrieve, delete).
- Retrieves all images or a single image with signed URLs.

### 🗄️ **Database Management**

- Uses **Prisma ORM** for schema management and database interactions.
- Utilizes **AWS RDS** MySQL for reliable and scalable database storage.
- Fetches data from cache or queries the database when necessary.

### 🚗 **Vehicle and Publication Management**

- Retrieves vehicles (bike, boat, car, RV) enriched with signed image URLs.
- Manages vehicle records:
  - Creates, updates, or deletes vehicles with specific details.
- Manages ads:
  - Creates new ads and updates related vehicles and subscriptions.
  - Retrieves ads with filtering, sorting, and pagination.
  - Handles ad statuses (inactive, deleted).
  - Calculates ad expiration dates based on subscription details.
  - Signs vehicle images for ad-related use cases.
- Provides counts of active ads by vehicle group.
- Renews corporate ads based on subscription updates.

### 💳 **Subscription Management**

- Creates and updates subscriptions with accurate expiration handling.
- Processes payments via **PayPal** and **Braintree** for credit cards.
  - Initiates PayPal orders and captures payments.
  - Generates OAuth2 access tokens for PayPal integration.

### 📍 **Profile and Address Management**

- Updates user attributes (e.g., phone, company description, etc.).
- Retrieves, creates, or deletes corporate user addresses.

### 🚚 **Vehicle Services (Bike, Boat, Car, RV)**

- Retrieves lists of vehicles by type, enriched with signed image URLs.
- Creates new vehicle records with required details.
- Updates or deletes specific vehicle records.

### 📊 **Additional Features**

- Retrieves vehicle attributes (fuel types, brands, transmissions, usage types) with active vehicle counts.
- Optimized performance using **Redis** caching.
- Provides health check endpoints for monitoring application status (basic and verbose).

<br>

## 🚀 Deployment

<br>

|  **Frontend**  |      **Backend**       |
| :------------: | :--------------------: |
| GitHub Actions |     GitHub Actions     |
|       S3       | AWS Lightsail (Docker) |
|   CloudFront   |       CloudFront       |

<br>

## 🙌 My Development Contributions

### Backend Development

- Designed and implemented REST APIs.
- Architected the database and managed data flows.

### CI/CD

- Automated builds and deployments using GitHub Actions.

### AWS Integration

- Configured and integrated **AWS services**.

<br>

## 🎨 UI & UX Design and Frontend

The user interface was developed following **Figma** designs provided by our team's **UI/UX Designer**.

<br>

## 👥 Team

[LinkedIn](https://www.linkedin.com/in/daniel-agray-rodriguez) **Daniel Agray Rodriguez** | UI & UX Design

[LinkedIn](https://www.linkedin.com/in/mychel-garzon-trujillo) **Mychel Garzon Trujillo** | Project Management and Frontend Development

[LinkedIn](https://www.linkedin.com/in/pinja-alanne-3920a1161) **Pinja Alanne** | Frontend Development

[LinkedIn](https://www.linkedin.com/in/doratokai28) **Dóra Tokai** | Frontend Development

[LinkedIn](https://www.linkedin.com/in/aj-kivimaki) **Atte Kivimäki** | Backend Development

<br>

## 📧 Contact

Feel free to reach out for any questions

[LinkedIn - Atte Kivimäki](https://www.linkedin.com/in/aj-kivimaki)
