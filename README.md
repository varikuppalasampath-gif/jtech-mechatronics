# Jtech website (React + Node.js)

Stack: React 18 + Vite (frontend), Express (backend API + static hosting), Zod validation, Nodemailer.

## Run locally
    npm install
    npm run dev          # starts API (:3000) and site together

## Deploy (needs a Node.js host)
    npm install
    npm run build
    cp .env.example .env   # fill SMTP details
    npm start              # serves site + /api/enquiry on PORT (default 3000)

Hosts that run Node: Render, Railway, DigitalOcean/AWS VPS, or GoDaddy VPS / cPanel "Setup Node.js App".
The GoDaddy Starter shared plan cannot run Node.js.
Without SMTP settings, enquiries are saved to server/enquiries.jsonl.
Pages: Home, About Us, Products, Services, Industries, Projects / Gallery, Careers, Contact Us (src/App.jsx, arrays at the top). Logo: public/logo.png.
