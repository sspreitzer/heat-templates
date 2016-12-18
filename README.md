# heat-templates

A collection of OpenStack Heat templates for various purposes and Red Hat
product testing.

## Prepare once

After cloning the repository:
```bash
$ virtualenv venv
$ source ./venv/bin/activate
(venv)$ pip install -U -r requirements.txt
```

## Activate
Before each session
```bash
$ source ./venv/bin/activate
(venv)$
```

## Deactivate
After session ended
```bash
(venv)$ deactivate
$
```

## Create credentials file
tbd

## List deployed stacks
```bash
(venv)$ openstack stack list
```

## Create a stack
```bash
(venv)$ openstack stack create --wait -e environmentfile -t templatefile stackname
```

## Delete a stack
```bash
(venv)$ openstack stack delete --yes --wait stackname
```
