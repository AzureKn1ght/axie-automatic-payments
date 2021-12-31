# Axie Automatic Payments

A fork of Axie Scholars Utilities

# How to Use

*   Create a folder called "files"

```
axie-scholar-utilities/docker/files
```

*   Download or create "payments.json" and put it in "files"

```
https://tracker.axie.management/payments
```

*   Open terminal in "axie-scholar-utilities/docker" and generate the "secrets.json" file

```
docker-compose run scholar-utilities generate_secrets files/payments.json files/secrets.json
```

*   Claim all the SLP for all accounts (open terminal in "axie-scholar-utilities/docker")

```
docker-compose run scholar-utilities claim files/payments.json files/secrets.json
```

*   Do all the payments automatically, or 1 by 1. (open terminal in "axie-scholar-utilities/docker")

```
docker-compose run scholar-utilities payout files/payments.json files/secrets.json -y
```
