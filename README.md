# ec2-instance-connect-cli

[aws-ec2-instance-connect-cli](https://github.com/aws/aws-ec2-instance-connect-cli) written in bash.

# Requirements
 - awscli
 - openssh (for ssh-keygen utility)

# Usage:

```
mssh [SSH_OPTIONS] [USER@]INSTANCE_ID
```

Examples:

```bash
# simple case
$ mssh i-xxxxxxxxxxxx

# specify user name
$ mssh ubuntu@i-xxxxxxxxxxxx

# add ssh options
$ mssh -v -p 8022 i-xxxxxxxxxxxx

# use non-default AWS profile
$ AWS_PROFILE=dev mssh ubuntu@i-xxxxxxxxxxxx
```

