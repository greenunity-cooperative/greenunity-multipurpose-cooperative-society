Greenunity Multipurpose Cooperative Society

A modern cooperative management platform designed to help Greenunity Multipurpose Cooperative Society manage members, savings, shares, loans, repayments, transactions, and cooperative administration from one secure application.

🌐 Production

Website: https://greenunity.online
Email: greenunitycooperativeonline@gmail.com

✨ Features

Member Management

- Member registration and login
- Unique cooperative member ID
- Member profile
- KYC status
- Next-of-kin information
- Member account status

Savings & Contributions

- Member savings accounts
- Contribution posting
- Contribution history
- Transaction references
- Account balance tracking

Shares

- Share account management
- Share balance tracking
- Share transactions

Loans

- Loan applications
- Loan amount and term
- Interest-rate recording
- Loan approval/rejection workflow
- Loan status tracking
- Repayment structure

Administration

- Administrator dashboard
- Member management
- Loan management
- Contribution posting
- Staff roles
- Audit logs

Security

- JWT authentication
- Password hashing with bcrypt
- Role-based access control
- Financial transaction ledger
- Audit logging
- PostgreSQL database

🏗️ Technology Stack

- Backend: Node.js
- Framework: Express.js
- Database: PostgreSQL
- Authentication: JWT
- Password Security: bcrypt
- Frontend: HTML, CSS, JavaScript
- Hosting: Render
- Source Control: GitHub

📁 Project Structure

greenunity-multipurpose-cooperative-society/
│
├── database/
│   └── schema.sql
│
├── public/
│   ├── index.html
│   ├── app.js
│   ├── styles.css
│   └── robots.txt
│
├── .env.example
├── .gitignore
├── package.json
├── server.js
├── render.yaml
├── README.md
└── DEPLOY-RENDER.md

🚀 Local Installation

1. Clone the repository

git clone https://github.com/YOUR_USERNAME/greenunity-multipurpose-cooperative-society.git
cd greenunity-multipurpose-cooperative-society

2. Install dependencies

npm install

3. Create PostgreSQL database

Create a PostgreSQL database named:

greenunity

Then run:

database/schema.sql

against the database.

4. Configure environment variables

Copy:

.env.example

to:

.env

Configure:

PORT=3000
DATABASE_URL=your_postgresql_connection_string
JWT_SECRET=your_long_random_secret

5. Start the application

npm start

Open:

http://localhost:3000

☁️ Render Deployment

The project includes:

render.yaml

for Render deployment.

Recommended architecture:

GitHub
   │
   ▼
Render Web Service
   │
   ├── Node.js / Express
   │
   └── Render PostgreSQL
            │
            ▼
       Greenunity App

After deployment, configure the custom domain:

greenunity.online

Render will provide the DNS records required for domain verification.

🔐 Environment Variables

Never commit production secrets to GitHub.

Required variables include:

DATABASE_URL=
JWT_SECRET=
NODE_ENV=production
APP_URL=https://greenunity.online
COOPERATIVE_EMAIL=greenunitycooperativeonline@gmail.com

🔎 Health Check

The application provides:

/api/health

Example:

curl https://greenunity.online/api/health

The endpoint should report that the application and database are available.

👥 User Roles

The application supports:

Role| Purpose
Member| Manage personal cooperative account
Loan Officer| Review and process loan applications
Treasurer| Manage financial transactions
Admin| Manage the entire cooperative platform

💰 Financial Controls

Financial operations should be recorded as ledger transactions rather than simply changing displayed balances.

Each financial transaction should have:

- Unique reference
- Member association
- Account type
- Transaction type
- Amount
- Direction
- Timestamp
- Creator
- Audit record

🔒 Production Security

Before processing real member funds, configure and verify:

- HTTPS
- Strong production secrets
- Database backups
- Rate limiting
- Input validation
- Payment webhook verification
- Administrative access controls
- KYC/AML procedures applicable to the cooperative
- Financial reconciliation
- Monitoring and logging
- Independent security testing

📧 Cooperative Contact

Greenunity Multipurpose Cooperative Society

Email:

"greenunitycooperativeonline@gmail.com"

Website:

"https://greenunity.online"

📄 License

Copyright © Greenunity Multipurpose Cooperative Society.

Use, modification, and redistribution should be governed by the organization's chosen licensing and ownership terms.

---

Greenunity Multipurpose Cooperative Society
Building stronger communities through cooperative savings, investment and financial participation.
