# Задание 2: Проектирование REST API

## Описание
Интернет-магазину "Петрушка Зеленая" нужен новый экран для отображения магазинов-партнеров с доставкой.  
При клике на карточку магазина должен осуществляться переход на внешний ресурс.

## Макет
<img width="380" height="759" alt="image" src="https://github.com/user-attachments/assets/838e89bd-a00f-4e61-9092-6c285edf9ff5" />

## Решение

### REST API запрос
При переходе пользователя на данный экран вызывается следующий запрос:
GET /api/v1/delivery/shops


### Пример ответа (JSON)
```json
{
  "shops": [
    {
      "id": "0001",
      "name": "METRO",
      "delivery_range_min": 21,
      "delivery_range_max": 23,
      "delivery_unit": "hours",
      "logo_url": "https://cdn.petrushka.ru/logos/metro.png",
      "deep_link": "https://partner.shop.ru/metro"
    },
    {
      "id": "0002",
      "name": "Ashan",
      "delivery_range_min": 18,
      "delivery_range_max": 20,
      "delivery_unit": "hours",
      "logo_url": "https://cdn.petrushka.ru/logos/ashan.png",
      "deep_link": "https://partner.shop.ru/ashan"
    },
    {
      "id": "0003",
      "name": "VkysVill",
      "delivery_range_min": 20,
      "delivery_range_max": 30,
      "delivery_unit": "minutes",
      "logo_url": "https://cdn.petrushka.ru/logos/vkysvill.png",
      "deep_link": "https://partner.shop.ru/vkysvill"
    },
    {
      "id": "0004",
      "name": "VICTORIA",
      "delivery_range_min": 17,
      "delivery_range_max": 19,
      "delivery_unit": "hours",
      "logo_url": "https://cdn.petrushka.ru/logos/victoria.png",
      "deep_link": "https://partner.shop.ru/victoria"
    }
  ]
}
