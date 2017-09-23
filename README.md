An Ansible role to configure PostgreSQL upstream [YUM repo](https://download.postgresql.org/pub/repos/yum/).

### Dependencies
None

### Tested Environment
* Ansible 2.3
* CentOS 7

### Installation

```
ansible-galaxy install rhops.postgresql-repo
```

### Role Variables
All the available options are not mandatory at the moment and they are subject to the structure of the official repo. So the variables are not able to work as expected, refer to the [original repo](https://download.postgresql.org/pub/repos/yum/).
Default values could be  referenced from the [role's defaults directory](defaults/main.yml).

* Switch PostgreSQL version

```
postgresql_version: 9.6
```

Validate values include `9.6`, `9.5`, `9.3`, `9.2`, `9.1`, `9.0` and `8.4`.

* PostgreSQl short version

```
postgresql_short_version: 96
```

This variable is for GPG key import and validate values include `96`, `95`, `93`, `92`, `91`, `90` and `84`.


* PostgreSQL repo host

```
postgresql_repo_host: https://download.postgresql.org/pub
```

This is used to configure repo mirror—`https://mirrors.tuna.tsinghua.edu.cn/postgresql`, for example.


* Enable PostgreSQL repo by default

```
postgresql_repo_enabled: "yes"
```

### License
Apache 2.0

### Author Information

This role was created in 2017 by [Jeff Li](https://blog.jeffli.me)
