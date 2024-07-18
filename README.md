# nextjs-dashboard
This is a dashboard written in Next.js hosted on Vercel, here's how you can try it out: 

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/dominikgorczyca/nextjs-dashboard
    cd nextjs-dashboard
    ```

2. **Set Up Database on Vercel**:
    - Go to [Vercel](https://vercel.com/).
    - Create a new PostgreSQL database.
    - Once the database is created, copy the database connection details.

3. **Set Up Environment Variables**:
    Create a `.env.local` file in the root directory and add the following:
    ```plaintext
    POSTGRES_URL="************"
    POSTGRES_PRISMA_URL="************"
    POSTGRES_URL_NO_SSL="************"
    POSTGRES_URL_NON_POOLING="************"
    POSTGRES_USER="************"
    POSTGRES_HOST="************"
    POSTGRES_PASSWORD="************"
    POSTGRES_DATABASE="************"
    AUTH_SECRET=your-secret-key
    AUTH_URL=http://localhost:3000/api/auth
    ```
    Replace the `************` with the actual connection details from Vercel and `your-secret-key` with your actual secret key.

4. **Install Dependencies**:
    Since the project uses the canary version of Next.js, you need to force the installation:
    ```bash
    npm install --force
    ```

5. **Run the Development Server**:
    Start the Next.js development server with:
    ```bash
    npm run dev
    ```

6. **Seed the Local Database**:
    After running the development server, open a browser and navigate to `http://localhost:3000/seed` to seed the database.

7. **Access the App**:
    Open a browser and navigate to `http://localhost:3000` to view the app.

### Login Credentials:
- **Email**: user@nextmail.com
- **Password**: 123456

