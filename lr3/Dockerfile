# Використовуємо офіційний образ nginx як базовий
FROM nginx

# Видаляємо файли за замовчуванням з папки /usr/share/nginx/html
RUN rm -rf /usr/share/nginx/html/*

# Копіюємо наш index.html до nginx-контейнера
COPY ./index.html /usr/share/nginx/html

# Відкриваємо порт 80 для доступу до веб-сервера
EXPOSE 80

# Запускаємо nginx
CMD ["nginx", "-g", "daemon off;"]
