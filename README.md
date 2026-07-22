# Custom HTML Views & Configurations for Home Assistant

Welcome to the **HTML Views for Home Assistant** repository! 

This project provides a collection of lightweight, standalone HTML views and corresponding JSON configuration files designed to embed seamlessly into web browsers on smart remote devices.

By keeping UI layouts rendered via HTML/JSON served directly from your Home Assistant local web server (`/config/www/`), you get fast, smooth updates without heavy dashboard overhead.

---

## 📋 Overview of HTML files

| File / View           | Type        | Category    | Description                                                        |
|:--------------------- |:----------- |:----------- |:------------------------------------------------------------------ |
| **`clock.html`**      | View        | Clock       | Analog flip clock                                                  |
| **`clock-face.html`** | View        | Clock       | Clock face                                                         |
| **`weather.html`**    | View        | Weather     | Daily weather forecast                                             |
| **`alarms.html`**     | View        | Alarms      | Alarm panel showing upcoming alarms.                               |
| **`shopping.html`**   | View        | TODO        | Large view shopping list                                           |
| **`bing.html`**       | View        | Screensaver | Bing's screensaver shows entire archive from 2019 to date          |
| **`switch.html`**     | Interactive | Media       | 6 switch interface . Allow configuration of switch name and icon   |

---

## 🚀 Installation & Setup

1. Connect to your Home Assistant server using **Samba Share**, **SSH/SFTP**, or the **File Editor** add-on.
2. Navigate to your `/config/www/` directory (if the `www` folder doesn't exist inside `/config/`, create it).
3. Copy html and respective json file to www or subfolder.
4.  If HTML card requires access to Home Assistant create long lived token. Save to token.txt. Copy file to same location as HTML. Once HTML loads file can be deleted.
5.  edit *__config.json file to add required data.
6.  Use Webpage card  or  web browser to view http://(ip of home assisistant):8123/local/clock.html
