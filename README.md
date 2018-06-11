alpha-cli
=========

`alpha-cli` provides a curl-like CLI wrapper around the `alpha` client. This
allows Lambda services to be directly invoked manually.

# Setup

```bash
$ npm install -g @lifeomic/alpha-cli
```

# Usage

```bash
$ alpha --help
Options:
  --help         Show help                                             [boolean]
  -H, --header   Pass custom header line to server
  -X, --request  Specify the request method to use
  --data-binary  Send binary data
  -V, --version  Show the version number and quit                      [boolean]

$ alpha lambda://user-service/users/jagoda | jq
{
  "id": "jagoda",
  "profile": {
    "email": "jeff.jagoda@lifeomic.com"
  }
}
```
