Follow the instructions [here](https://docs.duckietown.com/daffy/opmanual-duckiebot/setup/setup_laptop/index.html) to setup your computer. However, here are some troubleshooting tips if those instructions don't work.

If running ```docker run hello-world``` results in a permissions error, the following work-around fixes the issue for the current terminal session:

```
sudo groupadd -f docker
sudo usermod -aG docker $USER
newgrp docker
```

If  running ```which dts``` fails to output anything, you may need to export the path of the ```dts``` command to your terminal. Run the following command:

```
export PATH=$PATH:/home/{yourUserHere}/.local/bin
```

You may have to run this command each time you open a new terminal.

If that still doesn't work, try re-installing the duckietown-shell with this alternative command:

```
pip3 install --no-cache-dir --user -U duckietown-shell
```
