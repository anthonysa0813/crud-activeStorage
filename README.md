# crud & activeStorage (imágenes)

1. Instalar el active storage

```
 rails active_storage:install
```

2. Hacer un migrate

- Esto va a crear todo lo necesario y luego debemos de hacer un migrate

```
  rails db:migrate
```

3. crear una relación en el modelo

```ruby
class Product < ApplicationRecord
  has_one_attached :photo
  validates :title, :description, :price , presence: true
end
```
