![home2-thumbnail.png](https://github.com/kkamara/premium-artist-cms-template/raw/main/premium-artist-cms-theme/home2-thumbnail.png)

![01_image.png](https://github.com/kkamara/premium-artist-cms-template/raw/main/premium-artist-cms-theme/preview/01_image.png)

![showreel.png](https://github.com/kkamara/premium-artist-cms-template/raw/main/premium-artist-cms-theme/showreel.png)

![headshots.png](https://github.com/kkamara/premium-artist-cms-template/raw/main/premium-artist-cms-theme/headshots.png)

![admin.png](https://github.com/kkamara/premium-artist-cms-template/raw/main/premium-artist-cms-theme/admin/admin.png)

![dashboard.png](https://github.com/kkamara/premium-artist-cms-template/raw/main/premium-artist-cms-theme/admin/dashboard.png)

# Premium Artist CMS Template

Artist - Laravel 7 & Bootstrap 4 Performer's Portfolio CMS Template.

* [Installation](#installation)

* [Usage](#usage)

* [Configure Admin User](#configure-admin-user)

* [License](#license)

## Installation
* [https://laravel.com/docs/7.x/installation](https://laravel.com/docs/7.x/installation)
* [https://laravel.com/docs/7.x/mix#main-content](https://laravel.com/docs/7.x/mix#main-content)

```bash
cp .env.example .env
composer i
php artisan migrate --seed
```
## Usage

```bash
php artisan serve
# http://localhost:8000
# http://localhost:8000/admin
```

## Configure Admin User

```bash
php artisan tinker
```

```php
// default password: secret
factory(\App\User::class)->create(['name'=>'Kelvin Kamara','email'=>'kamaracomputers@gmail.com'])
User::all()
$u=App\User::find(1)
// roles: super admin, page admin, user admin
$u->assignRole('super admin')
$u->save()
```

## Misc

<p>I built Premium Artist CMS Template in four weeks back in early 2020.</p>

## License
[Legal](https://themeforest.net/legal/author#how-selling-your-items-works)
