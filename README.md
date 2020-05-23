# Laravel Lumen 5.x Scaffold Generator
## Usage

### Step 1: Install Through Composer

```
composer require ycamposde/xfscaffold:dev-master --dev
```
##### add:
```
"required": {
    ...
    ...
    "webpatser/laravel-uuid": "^3.0",
    "urameshibr/lumen-form-request": "^1.5"
}

```
### Step 2: Add the Service Provider

Open `config/app.php` and, to your **providers** array at the bottom, add:

```
$app->register(ycamposde\xfscaffold\GeneratorsServiceProvider::class);
```

### Step 3: Run Artisan!

You're all set. Run `php artisan` from the console, and you'll see the new commands `make:scaffold`.

## Examples

Use this command to generator scaffolding of **Example** in your project:
```
php artisan make:scaffold Example
```

This command will generate:

```
app/Models/Example.php
app/Http/Controllers/Api/ExampleController.php
app/Http/Request/ExampleStore.php
app/Repositories/Example.php
app/Services/Example.php
```


##Collaborators
 [Yerson Campos](https://github.com/ycamposde "ycamposde")