# Exporters installer for Ubuntu servers

Run the following command to install node exporter on your Ubuntu server:

```bash
bash <(curl -sSL https://github.com/ongtungduong/quick-installers/raw/main/node-exporter/install.sh)
```

**You can customize the installation by setting environment variables:**

- EXPORTER_VERSION: To install specific version of node exporter (default: latest)
- EXPORTER_PORT: To specify a custom port (default: 9100)

**For example, to use port 17017, run the following command:**

```bash
EXPORTER_PORT="17017" bash <(curl -sSL https://github.com/ongtungduong/quick-installers/raw/main/node-exporter/install.sh)
```
