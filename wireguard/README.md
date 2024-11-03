# Wireguard installer for Ubuntu servers

**Make sure that your kernel supports WireGuard (all modern kernels).**

## Usage

To install Wireguard and CLI, run the following command.

```bash
bash <(curl -sSL https://github.com/ongtungduong/installers/raw/main/wireguard/install.sh)
```

To uninstall Wireguard and CLI, run the following command.

```bash
bash <(curl -sSL https://github.com/ongtungduong/installers/raw/main/wireguard/uninstall.sh)
```

## SHC Compiler (Optional)

You can use SHC Compiler to convert the CLI script into a Binary Executable.

### Install SHC Compiler

```bash
sudo add-apt-repository ppa:neurobin/ppa
sudo apt-get update -y
sudo apt-get install shc -y
```

### Compile the CLI script

```bash
sudo curl -sSL https://github.com/ongtungduong/installers/raw/main/wireguard/wireguardcli.sh -o wireguardcli.sh
sudo chmod +x wireguardcli.sh
sudo shc -vrf wireguardcli.sh -o wireguardcli
sudo mv wireguardcli /usr/local/bin/wireguardcli
sudo rm wireguardcli.sh
```
