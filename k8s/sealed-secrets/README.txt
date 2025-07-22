# Sealed Secrets Directory

- Place your unsealed secret (e.g., mysecret.yaml) here temporarily.
- Do NOT commit mysecret.yaml to git.
- Use the following command to generate a sealed secret:

  kubeseal --cert pub-cert.pem -o yaml < mysecret.yaml > mysealedsecret.yaml

- Commit only mysealedsecret.yaml to git. 