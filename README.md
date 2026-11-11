# Ollama 

Instala Ollama mediante el script oficial:

```bash
curl -fsSL https://ollama.com/install.sh | sh
```

---

## Paquete ROCm

Si necesitas la versión para AMD/ROCm, descarga y descomprime el paquete directamente en `/usr`:

```bash
curl -fsSL https://ollama.com/download/ollama-linux-amd64-rocm.tar.zst | sudo tar --zstd -x -C /usr
```

---

## Iniciar el servicio

Inicia el servicio de Ollama:

```bash
sudo systemctl start ollama
```

Comprueba su estado:

```bash
sudo systemctl status ollama
```

---

## Servicio automático

Para iniciar Ollama automáticamente al arrancar el sistema:

```bash
sudo systemctl enable ollama
```

---

## Ejecutar un modelo

Para descargar y ejecutar `llama3.2`:

```bash
ollama run llama3.2
```

---
