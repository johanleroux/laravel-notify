# Flexible flash notifications for Laravel

## Install
```
composer require johanleroux/laravel-notify
```

##  Usage
```php
notify()->flash('Welcome back!', 'success');

notify()->information('Welcome back!');

notify()->success('Profile updated!');

notify()->warning('Invalid Data!');

notify()->danger('User Deleted!');
```

Within a view, you can now check if a flash message exists and output it.
```php
@if (notify()->ready())
    <div class="alert-box {{ notify()->type() }}">
        {{ notify()->message() }}
    </div>
@endif
```

## Issues and contribution
Just submit an issue or pull request through GitHub. Thanks!

## License
The MIT License (MIT). Please see [License File](LICENSE.md) for more information.