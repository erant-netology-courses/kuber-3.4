# kuber-3.4

## Задание 1

1. Rolling update - не подходит т.к. новые версии не могут общаться со старыми, что может породить несогласованность данных и обмена информацией между сервисами.
1. **Recreate - лучший вариант, нет пересечения между версиями. Простой - компенсация отсутствия ресурсов.**
1. Blue-green, Canary и A/B tests - не подходят, т.к. ресурсов больше не выделят, а общий запас всего 20%.

## Задание 2

Обновление с полной доступностью:

<img width="1060" height="1060" alt="image" src="https://github.com/erant-netology-courses/kuber-3.4/blob/main/2_2.jpg?raw=true" />

ДЗ устарело, nginx:1.28 уже существует:

<img width="1060" height="1060" alt="image" src="https://github.com/erant-netology-courses/kuber-3.4/blob/main/2_3_fail.jpg?raw=true" />

Накатил nginx:1.38, откатил обратно:

<img width="1060" height="1060" alt="image" src="https://github.com/erant-netology-courses/kuber-3.4/blob/main/2_4.jpg?raw=true" />