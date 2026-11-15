# Bot de Telegram: cifrado César y cadenas de Markov

Entrega 03 de Estructuras Discretas, Universidad del Norte.

Bot disponible en: https://t.me/Iso_Morfos_jr_bot

## Archivos

- `bot.py`: comandos del bot, menú y arranque.
- `cesar.py`: cifrado y descifrado César con un alfabeto de 73 caracteres.
- `markov.py`: modelo de Markov de orden K, generación de texto y frecuencias.
- `scraper.py`: descarga del texto plano de un sitio web estático.
- `requirements.txt`: librerías necesarias.

## Requisitos

- Python 3.10 o superior.
- Un token de bot de Telegram (se obtiene con @BotFather).

## Instalación

1. Instalar las librerías:

   ```
   pip install -r requirements.txt
   ```
Para obtener un token: abrir @BotFather en Telegram, enviar /newbot,
elegir un nombre y un usuario que termine en "bot", y copiar el token
que entrega.

2. Crear en esta misma carpeta un archivo llamado `.env` con una sola línea:

   ```
   TELEGRAM_TOKEN=aquí_va_el_token_del_bot
   ```

3. Ejecutar el bot:

   ```
   python bot.py
   ```

El bot responde mientras el programa esté en ejecución.

## Comandos

| Comando | Función |
|---|---|
| `/ayuda` | Describe el bot y sus comandos |
| `/cifrar <desplazamiento> <mensaje>` | Cifra con César |
| `/descifrar <mensaje>` | Descifra sin conocer el desplazamiento |
| `/scrapear <url>` | Descarga el texto de un sitio estático |
| `/markov <K> <N>` | Genera N caracteres con un modelo de orden K |
| `/histograma <K>` | Histograma de frecuencias de las K-tuplas |
| `/menu` | Menú con botones para alternar entre histograma y generar texto |

El archivo `.env` no se incluye en la entrega porque contiene el token.
