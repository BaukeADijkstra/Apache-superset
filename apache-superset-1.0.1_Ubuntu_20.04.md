## **How to install Apache-superset-1.0.1 on Ubuntu-20.04-LTS**

##### Dependencies

```
sudo apt update
sudo apt upgrade
sudo apt-get install build-essential libssl-dev libffi-dev python3-dev python3-pip libsasl2-dev libldap2-dev
```

 **virtual environment**

```
sudo apt-get install python3-venv
```

**Create and activate VE**

```
python3 -m venv superset-env
```

```
source superset-env/bin/activate
```

**Install superset**

```
pip install apache-superset
```

##### Initializing database 

```
superset db upgrade
```

**Create default role and permissions**

```
superset init
```

**admin user create**

```
superset fab create-admin
```

**Load examples**

```
superset load_examples
```

**Run server on 8080**

```
superset run -p 8080 -h 0.0.0.0
```
