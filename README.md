<h1 align="center">enum_oblako</h1>
<div align="center">
  S3/SAAS enumerator
  <br>
  <br>
  <img alt="Static Badge" src="https://img.shields.io/badge/python-3.10+-blue.svg">
  <img alt="Static Badge" src="https://img.shields.io/badge/tested%20on-Linux-blue.svg">
  <p></p>
  <a href="https://github.com/lisp3r/enum_oblako?tab=readme-ov-file#Installation">Install</a>
  <span> • </span>
  <a href="https://github.com/lisp3r/enum_oblako?tab=readme-ov-file#Enum%20S3%20buckets%20and%20SaaS">Documentation</a>
  <span> • </span>
	<a href="https://github.com/lisp3r/enum_oblako?tab=readme-ov-file#usage">Usage</a>
  <p></p>
</div>

## Enum S3 buckets and SaaS

For now enum_oblako supports following services:

- Slack
- Atlassian
- Salesforce
- Yandex Gitlab
- Yandex Website
- Yandex Cloud S3
- VK Cloud S3
- Croc Cloud S3
- Selectel Cloud S3
- MTS Cloud S3
- Sbercloud S3
- Scaleway S3
- Exoscale S3
- OVHCloud S3
- Ionos S3
- Linode S3
- Vultr S3
- Digital Ocean S3

Enum_oblako can be run in two modes:
- Generate and enum (generate namespaces and bucketnames for you based on company's name)
- Enum (run enumeration based on submitted namespaces' and buckets' files)

## Usage

```sh
$ enum_oblako --generate --name <target name> --rps 100
```

It generates a list of mutations based on the target's name and the wordlists (`namespaces.txt`, `buckets.txt`).

You can also supply you own wordlists:

```sh
$ enum_oblako --namespaces my_namespaces.txt --buckets my_buckets.txt --name <target name> --rps 100
```

It supports two regions: ru and eu (or all if you want both):

```sh
$ enum_oblako --generate --name <target name> --region eu --rps 100
```

## Installation

### From Git

```sh
$ git clone https://github.com/lisp3r/enum_oblako.git
$ cd enum_oblako
~/enum_oblako $ python -m venv .venv
~/enum_oblako $ source .venv/bin/activate
~/enum_oblako $ pip install -r requirements.txt
~/enum_oblako $ python enum_oblako --help
```

### Using PIP

```bash
$ python -m pip install https://github.com/etyvrox/enum_oblako/releases/latest/download/enum-oblako.tar.gz
```

:sleeping: pip is not supported
