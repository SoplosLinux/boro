# 📦 Repositorio APT oficial de Soplos Linux Boro

Repositorio APT oficial de Soplos Linux Boro

## 🛠️ Instalación

### 1️⃣ Añadir la clave GPG
```bash
# Descargar e instalar la clave GPG
sudo mkdir -p /usr/share/keyrings
wget -qO - https://raw.githubusercontent.com/SoplosLinux/boro/main/public.key | sudo gpg --dearmor -o /usr/share/keyrings/boro.gpg
```

### 2️⃣ Añadir el repositorio

```bash
# Añadir la fuente APT
echo "deb [signed-by=/usr/share/keyrings/boro.gpg trusted=yes] https://github.com/SoplosLinux/boro/raw/refs/heads/main/ stable main" | sudo tee /etc/apt/sources.list.d/boro.list

# Actualizar índices
sudo apt update --allow-insecure-repositories
```

### 3️⃣ Instalar paquetes

```bash
sudo apt install nombre-del-paquete
```

## 🔍 Buscar paquetes disponibles
Para ver todos los paquetes disponibles:

```bash
apt search boro
```

## 🔗 Links útiles

- [🌐 Sitio web](https://soplos.org)
- [📚 Documentación](https://soplos.org/wiki)
- [💬 Foro](https://soplos.org/forums)

## 🤝 Contribuir
¿Encontraste un error o tienes una sugerencia? ¡Abre un issue!

## 📝 Licencia
Este repositorio está bajo la licencia GPL-3.0.