# AmoCRM Kanban Integration

Интеграция между AmoCRM и канбан-доской для автоматического создания броней.

## 🚀 Быстрое развертывание на Vercel

### Шаг 1: Создайте репозиторий на GitHub
1. Перейдите на https://github.com
2. Нажмите "New repository"
3. Назовите: `amo-kanban-integration`
4. Сделайте Public
5. Создайте репозиторий

### Шаг 2: Загрузите файлы
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/amo-kanban-integration.git
git push -u origin main
```

### Шаг 3: Разверните на Vercel
1. Перейдите на https://vercel.com
2. Войдите через GitHub
3. Нажмите "New Project"
4. Выберите ваш репозиторий
5. Нажмите "Deploy"

### Шаг 4: Получите URL
После деплоя получите URL вида:
```
https://amo-kanban-integration-xxx.vercel.app
```

### Шаг 5: Настройте webhook в AmoCRM
Замените URL webhook на:
```
https://amo-kanban-integration-xxx.vercel.app/api/amo-webhook
```

## 📋 Что делает интеграция

1. **Получает данные** из AmoCRM через webhook
2. **Преобразует** сделку в формат брони
3. **Создает бронь** в канбан-доске автоматически

## 🔧 Настройка полей в AmoCRM

Создайте пользовательские поля в сделках:
- **Имя Брони** - имя клиента
- **Дата и время брони** - время брони
- **Кол-во гостей** - количество гостей
- **Зона** - выбранная зона
- **Филиал** - филиал (Московское шоссе 43 = МСК)
- **Коммент к брони** - комментарий

## 🧪 Тестирование

1. Создайте сделку в AmoCRM
2. Заполните все поля
3. Сохраните сделку
4. Проверьте канбан-доску - должна появиться новая бронь

## 📞 Поддержка

При возникновении проблем проверьте:
- Логи в Vercel Dashboard
- Правильность URL webhook
- Заполнение всех полей в сделке
