# Laravel Portfolio Setup Instructions

## What Was Converted

Your static HTML/CSS portfolio has been converted to Laravel with the following structure:

### Files Created:
- `resources/views/layouts/app.blade.php` - Main layout template
- `resources/views/partials/header.blade.php` - Navigation header
- `resources/views/partials/footer.blade.php` - Footer section
- `resources/views/home.blade.php` - Main home page with all sections
- `app/Http/Controllers/HomeController.php` - Controller with certificates data
- `routes/web.php` - Route configuration
- `public/css/style.css` - Your CSS file

## Setup Steps

1. **Move your image files** to `public/images/` directory:
   ```
   mkdir public\images
   move *.png public\images\
   move *.jpg public\images\
   ```

2. **Install Laravel** (if you haven't already):
   ```
   composer create-project laravel/laravel laravel-portfolio
   ```

3. **Copy the generated files** into your Laravel project

4. **Start the development server**:
   ```
   php artisan serve
   ```

5. **Visit** http://localhost:8000

## Key Changes Made

- Split HTML into Blade templates with layout inheritance
- Created a controller to manage certificate data dynamically
- Used Laravel's `@foreach` loop for certificates instead of hardcoded HTML
- Implemented `asset()` helper for proper asset URLs
- Organized views into layouts and partials for better maintainability

## Next Steps (Optional)

- Move certificates data to a database
- Add admin panel to manage certificates
- Implement contact form with email functionality
- Add authentication if needed
