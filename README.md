# download_pkg_and_deps

Script en Bash para **descargar un paquete Debian y sus dependencias** hasta un nivel de profundidad especificado.  
Útil cuando necesitas preparar repositorios locales, realizar instalaciones en sistemas sin Internet o analizar árboles de dependencias.

Autor: **Esteban M. Navas Martín**  
Última actualización: **23/11/2025**

---

## 📌 Características

- Descarga un paquete `.deb` desde los repositorios configurados.
- Descarga sus dependencias hasta un número de niveles definido por el usuario.
- Evita descargas repetidas gracias al control interno de paquetes procesados.
- Usa `apt-cache depends` para obtener dependencias reales del repositorio.
- Requiere privilegios de **root**.

---

## 📦 Sintaxis

```bash
sudo ./download_pkg_and_deps paquete [nivel_dependencia]
