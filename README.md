# Tango GraphQL Exercise

```shell
git clone https://github.com/HFRibeiro/web-maxiv-tangogql.git
git clone https://gitlab.com/MaxIV/python3-taurus-core.git
sudo apt-get update
sudo apt-get -y install build-essential
sudo apt-get -y install mysql-server mysql-client
sudo apt-get -y install tango-db tango-common tango-test
/usr/lib/tango/TangoTest test
```

### Open a new comand line
```bash
sudo apt-get -y install python3-pip
sudo apt-get -y install python3-pytango
cd python3-taurus-core
sudo python3 setup.py install
cd ../web-maxiv-tangogql
pip3 install -r requirements.txt
pip3 install PyJWT
python3 -m tangogql
```

### After this if you go to http://localhost:5004/graphiql/ you should see GraphiQL web interface

### Now start following the steps from: https://docs.google.com/document/d/1bgIS02F_c0k90x4cis6qFSyN0zO-fa9W8H-TF3gnShE


#### PS: From the origin repository from MAXIV I just changed one file, the tangogql/auth.py this file is listening to the mutation function and blocking it, i just change this to find for mutationXX.