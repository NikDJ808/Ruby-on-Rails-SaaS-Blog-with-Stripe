# SaaSBlog

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)

## Introduction

SaaSBlog is a Software-as-a-Service (SaaS) blogging platform built with Ruby on Rails. It provides a comprehensive solution for creating and managing a blog, with subscription-based access to premium content using Stripe for payment processing. This project aims to demonstrate a complete SaaS application with user authentication, content management, and payment integration.

## Features

- User authentication with Devise
- Subscription management with Stripe
- Blog post creation and management
- Static pages for general information
- Responsive design

## Technologies Used

- **Ruby on Rails**: The web application framework used for development.
- **PostgreSQL**: Database management system.
- **Devise**: Authentication solution for Rails.
- **Stripe**: Payment processing.
- **Webpacker**: For managing JavaScript assets.
- **Bootstrap**: For responsive design and styling.
- **RSpec**: For testing the application.

## Setup and Installation

### Prerequisites

Ensure you have the following installed on your local development environment:

- Ruby 3.0.0 or newer
- Rails 6.0.0 or newer
- PostgreSQL
- Node.js
- Yarn

### Installation Steps

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/saasblog.git
   cd saasblog
   ```

2. **Install dependencies:**

   ```bash
   bundle install
   yarn install
   ```

3. **Setup the database:**

   ```bash
   rails db:create
   rails db:migrate
   rails db:seed
   ```

4. **Set up Stripe:**

   - Add your Stripe API keys to your environment variables or a credentials file.

5. **Start the Rails server:**

   ```bash
   rails server
   ```

6. **Visit the application:**

   Open your web browser and go to `http://localhost:3000`.

## Usage

Once the application is up and running, you can:

- Sign up for a new account.
- Create and manage blog posts.
- Subscribe to premium content.
- View and edit your subscription settings through the billing portal.

## Folder Structure

Here is an overview of the main directories and files in the project:

```
saasblog/
├── app/
│   ├── assets/
│   │   ├── config/
│   │   ├── images/
│   │   └── stylesheets/
│   ├── channels/
│   ├── controllers/
│   ├── helpers/
│   ├── javascript/
│   ├── jobs/
│   ├── mailers/
│   ├── models/
│   ├── views/
│   └── channels/
├── bin/
├── config/
│   ├── environments/
│   ├── initializers/
│   ├── locales/
│   └── application.rb
├── db/
│   ├── migrate/
│   ├── schema.rb
│   └── seeds.rb
├── lib/
├── log/
├── public/
├── test/
├── tmp/
├── vendor/
├── Gemfile
├── Gemfile.lock
├── Rakefile
├── config.ru
└── README.md
```
