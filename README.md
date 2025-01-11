<details><summary>connector</summary>

  ```sh
  # Available versions:
  # * 6.2.0
  # 
  # Create command:
  # --------------
  # tar -czf - CONNECTOR... | age -e -r age1n2mrmmquny3f0z056fhv4yl4ydf7heuaxq2nkqyxs9shlg7checqtmgtv2 > ./connector-VERSION.tgz.age
  curl -fsSL https://github.com/spaghetti-coder/linux-helper-secrets/raw/connector/connector-6.2.0.tgz.age \
  | age -d -i <(base64 -d < age-key.age.base64 | age -d) \
  | (tmp="$(set -x; mktemp -d)"; set -x; tar -xzf - -C "${tmp}")
  ```
</details>
