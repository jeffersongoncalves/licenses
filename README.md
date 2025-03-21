# ⚠️ Disclaimer

This package management system is provided "as is" without warranty of any kind, either expressed or implied, including but not limited to the implied warranties of merchantability and fitness for a particular purpose. The entire risk as to the quality and performance of the software is with you.

By using Satis Package Manager, you acknowledge that:

1. The creators and contributors of this project shall not be held liable for any damages, including but not limited to, direct, indirect, special, incidental, or consequential damages or loss of data resulting from the use or inability to use this software.

2. You are responsible for ensuring that your use of this package management system complies with all applicable laws, regulations, and license agreements of the packages you manage through it.

3. This tool does not guarantee the security, quality, or legality of any third-party packages it may help you manage or distribute.

4. You will exercise appropriate caution when using this system in production environments and implement proper security measures.

Use at your own risk.

# SatisUI Package Manager

A Filament application for managing PHP packages using Satis.

## About

This project is a complete package management system built around Satis using FilamentPHP as the backend. It provides tools for creating, managing, and distributing PHP packages within organizations or communities.

## Requirements

- PHP 8.2+
- Laravel 12.x
- Node.js & NPM
- Composer
- Git

## Features

- Private package repository management
- Package versioning
- Access control and user permissions
- Web interface for repository management

## Installation

1. Clone the repository:
```bash
git clone https://github.com/filamentphp-br/satis.git
```

2. Install PHP dependencies:
```bash
composer install
```

3. Install JavaScript dependencies:
```bash
npm install
```

4. Copy the environment file:
```bash
cp .env.example .env
```

5. Generate application key:
```bash
php artisan key:generate
```

6. Configure your database in the `.env` file

7. Run migrations:
```bash
php artisan migrate
```

8. Build assets:
```bash
npm run dev
```

## Configuration

The system can be configured through the web interface or by editing the configuration files in the `config` directory.

### Setting Up Repositories

1. Navigate to the admin panel
2. Add your Git repositories with appropriate credentials
3. Configure build settings and access controls
4. Generate your package repository

## Usage

### Adding to Composer

To use this repository in your projects, add the following to your composer.json:

```json
{
    "repositories": [
        {
            "type": "composer",
            "url": "https://your-satis-url.com"
        }
    ]
}
```

### Managing Packages

- Use the web interface to manage packages and permissions
- Set up automation workflows through the API
- Monitor package usage and statistics

## Development

- For development: `npm run dev`
- For production build: `npm run build`

## Testing

Run the tests with:
```bash
php artisan test
```

## Packages Used

### PHP Packages
- Laravel Framework v12.1.0
- Laravel Sanctum v4.0.8
- Laravel Sail v1.41.0
- Composer/Satis
- PHPUnit for testing
- Mockery v1.6.12
- GuzzleHTTP v7.9.2
- Faker v1.24.1
- Monolog v3.8.1

### JavaScript Packages
- Axios v1.7.4
- Vite v6.0.11
- TailwindCSS v3.4.17
- PostCSS v8.5.3
