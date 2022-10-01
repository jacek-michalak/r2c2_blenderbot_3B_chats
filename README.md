After specifying the subject of the conversation AI talks to AI.

You can install it with:

```bash
# The best offline chatbot: r2c2_blenderbot_3B
# 16 GB on HDD (SSD recommended)
# Works with Ubuntu 20.04.4 (16 GB RAM and 16 GB swapfile)
# No GPU needed
# 
# In windows you can run it at:
# https://www.vmware.com/products/workstation-pro/workstation-pro-evaluation.html

sudo apt-get update
sudo apt install python3-pip

# If You have only 16 GB of RAM add 16 GB to swapfile
# If You have 32 GB of RAM skip this

sudo swapoff /swapfile  
sudo rm  /swapfile
sudo fallocate -l 16G /swapfile
sudo chmod 600 /swapfile
sudo mkswap /swapfile
sudo swapon /swapfile

# Main part

sudo pip install parlai
sudo parlai i -mf zoo:seeker/r2c2_blenderbot_3B/model




```
