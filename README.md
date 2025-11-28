# download_pkg_and_deps

## 📜 Overview

Script en Bash para **descargar un paquete Debian y sus dependencias** hasta un nivel de profundidad especificado.  
Útil cuando necesitas preparar repositorios locales, realizar instalaciones en sistemas sin Internet o analizar árboles de dependencias.

---

## 📌 Características

- Descarga un paquete `.deb` desde los repositorios configurados.
- Descarga sus dependencias hasta un número de niveles definido por el usuario.
- Evita descargas repetidas gracias al control interno de paquetes procesados.
- Usa `apt-cache depends` para obtener dependencias reales del repositorio.
- Requiere privilegios de **root**.

---

## 📦 Instalación

```bash
   wget --no-check-certificate -O /usr/local/sbin/download_pkg_and_deps https://github.com/algodelinux/download_pkg_and_deps/raw/master/download_pkg_and_deps  
   chmod 755 /usr/local/sbin/download_pkg_and_deps
```

---

## 🛠 Sintaxis

```bash
sudo ./download_pkg_and_deps paquete [nivel_dependencia]
```

---

## ✒️ Authors

**Esteban M. Navas Martín**  algodelinux@gmail.com

---
