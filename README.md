hola diego
PRIMERO EMPEZAMOS HACIENDO UN DOCKER BUILD
docker build -t flask-cat-app:papisanti .

DESPUES HACEMOS UN DOCKER RUN PARA PODER VERLO
docker run -p 8888:5000 flask-cat-app:papisanti

<img width="940" height="677" alt="Captura de pantalla 2025-10-24 153205" src="https://github.com/user-attachments/assets/96e830b2-6188-4a0c-89d9-e54f22a757da" />


EN EL CODIGO PONIA IMAGES Y AL LADO HACER UNA LISTA DE GIFT DE GATOS HEHE

Añadimos en nuestro compose.yml
services: web: build .ports: -"8888:5000"
