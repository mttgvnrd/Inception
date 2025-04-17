# 🐳 Inception - Dockerized Infrastructure  

**42 Firenze Project | System Administration**  
*Infrastruttura con NGINX, WordPress, e MariaDB containerizzati in Docker, conforme alle specifiche 42.*  

---

## 📋 Specifiche  
✅ **Stack**:  
   - `Docker` + `docker-compose`  
   - `NGINX` (TLSv1.2/1.3)  
   - `WordPress` + `php-fpm`  
   - `MariaDB`

✅ **Regole**:  
   - Immagini custom da Alpine/Debian (no pre-built)  
   - Volumi per database e file WordPress  
   - Rete Docker dedicata  
   - Restart automatico dei container

✅ **Sicurezza**:  
   - Variabili d'ambiente (`.env`)  
   - Niente password in chiaro nei Dockerfile  
   - Dominio personalizzato (`mgiovana.42.fr`)  

---

## 🛠 Installazione  
```bash
git clone https://github.com/mttgvnrd/Inception.git
cd Inception/project/srcs
make  # Avvia l'infrastruttura
