# Stable Diffusion XL

```sh
sudo apt install dotnet-sdk-7.0 git
wget https://github.com/cloudflare/cloudflared/releases/latest/download/cloudflared-linux-amd64.deb
sudo dpkg -i cloudflared-linux-amd64.deb
git clone https://github.com/Stability-AI/StableSwarmUI
cd StableSwarmUI/
bash ./launch-linux.sh --launch_mode none --cloudflared-path cloudflared --explicit_shell bash
```
