# AWS CDK GETTING STARTED


### 1. INSTALL AWS CLI AND CONFIGURE

- **ON LINUX or Windows with WSL**

```bash
$ curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

- **ON WINDOWS**

  [Click To Download and run the AWS CLI MSI installer for Windows (64-bit)](https://awscli.amazonaws.com/AWSCLIV2.msi)

### 2. CONFIRM INSTALLATION BY CHECKING YOUR CURRENT AWS VERSION

```bash
 aws --version
```

### 3. CONFIGURE YOUR MACHINE WITH YOUR CREDENTIALS AND AWS REGION

```bash
aws configure
```

- You will get prompts to provide your **_region(defult is use-east-1)_**, **_aws_access_key_id_** , **_aws_secret_access_key_**.

- For a more difinitive guide on AWS CONFIGURATION follow [this guide](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)

### 4. INSTALL AWS CDK GLOBALLY

- Check that you have **_node_** and **_npm_** installed if not installed [get it here](https://nodejs.org/en/download/)

```
node -v
npm -v
```

- Install AWS CDK Globally

```bash
npm i -g aws-cdk
```

### 5. INSTALL DOCKER (not necessary but nice to have)

- Follow the provided guides to get install and get started with docker.
- [On Windows](https://www.geeksforgeeks.org/how-to-install-docker-on-windows/)
- [On Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04)

## SAMPLE PROJECT

- Initialize an application
```bash
cdk init app --language typescript
```

- Synthesis the app to a cloudformation template
```bash
cdk synth > output.yaml
```

- Deploy your application
```bash
cdk deploy
```