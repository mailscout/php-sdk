## Tag

#### Get tags

```php
\Mailscout::setApiKey('YOUR_MAILSCOUT_API_TOKEN');

$tag = new \Mailscout\Tag();
$tag->retrieve();
```

#### Add a new tag

```php
$tag->add([
    'name' => 'my tag'
]);
```

#### Get an existing tag

```php
$tag->get(1);

// or

$tag->find(1);
```

#### Update an existing tag

```php
$tag->update(1, [
    'name' => 'my new tag'
]);
```

#### Remove tag

```php
// for deleting single tag
$tag->remove([1]);

// for deleting multiple tag
$tag->remove([1, 2, 3]);
```

#### Get all tags without pagination

```php
$tag->all()
```