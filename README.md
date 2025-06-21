# kccp – KDE Connect Copy

`kccp` is a lightweight POSIX-compliant shell script that allows you to easily share files with your connected KDE Connect devices via the command line. It supports both single file transfers and bulk transfers using regular expressions.

Enjoy fast file sharing from your terminal — no clicks needed.

---

## 📦 Features

- Share files with KDE Connect using `kdeconnect-cli`
- Supports both file paths and regex-based matching
- Multilingual help output (currently English and Spanish)
- Designed for minimal systems and fast execution

---

## ✅ Requirements

- KDE Connect
- `kdeconnect-cli` available in your `PATH`
- A POSIX-compatible shell (`sh`, `dash`, etc.)

---

## 📥 Installation

Copy the script somewhere in your `$PATH`, and make it executable:

~~~
# cp kccp /usr/local/bin/
# chmod +x /usr/local/bin/kccp
~~~
---

## 🖥️ Usage

~~~
$ kccp 'foto de perro.jpg' android
$ kccp '/.+\.jpg/' 'my device'
~~~

---

## 🛠️ Config (optional)

A default device can be configured.

~~~
$ mkdir ~/.config/kccp
$ echo default_device = nombre del dispositivo > ~/.config/kccp/kccprc
~~~

💡 Examples using the configured default device
~~~
$ kccp 'foto de perro.jpg'
$ kccp '/.+\.jpg/'
~~~
