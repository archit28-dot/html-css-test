# Landing Page - Nginx Virtual Host

A responsive landing page built using HTML and CSS, based on the provided design reference.

The project is served locally using an Nginx virtual host.

## Features

- Responsive landing page
- Desktop and mobile layouts
- Header navigation
- Hero section
- Information cards
- Quote/testimonial section
- Call-to-action section
- Footer
- Local Nginx virtual host configuration

## Technologies Used

- HTML5
- CSS3
- Nginx
- Git

## Project Structure

```text
archit-test/
├── images/
├── index.html
├── style.css
└── README.md
## HTTPS and SSL

The website is served locally using Nginx with a self-signed SSL certificate.

### Local URL

https://archit-test.local

HTTP requests are permanently redirected to HTTPS.

### Certificate Details

- **Certificate type:** Self-signed X.509 certificate
- **Algorithm:** RSA 2048-bit
- **Validity:** 365 days
- **Subject Alternative Name (SAN):** `DNS:archit-test.local`

### Certificate Files

The certificate and private key are stored outside the project repository:

- Certificate: `/etc/nginx/ssl/archit-test.local.crt`
- Private key: `/etc/nginx/ssl/archit-test.local.key`

The private key is not included in this Git repository.

### Nginx Configuration

The Nginx server configuration is located at `/etc/nginx/sites-available/archit-test`.

The configuration uses port 80 to redirect HTTP requests to HTTPS and port 443 to serve the website using the certificate and private key.

### Browser Warning

Because the certificate is self-signed, browsers may display a security warning until the certificate is explicitly trusted. This is expected for this local development setup.

The certificate provides encrypted HTTPS connections, but it is not automatically trusted by browsers or operating systems.
