# Local .terraform directories
**/.terraform/* - сопоставление всех каталогов выше папки .terraform (a/b/c/.terraform) и всех файлов в папке .terraform

# .tfstate files
*.tfstate - исключение всех файлов с расширением .tfstate
*.tfstate.* - все файлы tfstate с любым расширением (root@debian:/home/firewall/devops25-netology/terraform# git check-ignore -v 123.tfstate.123 terraform/.gitignore:6:*.tfstate.*      123.tfstate.123)

# Crash log files
crash.log - только crash.log
crash.*.log - любые файлы crash.*.log

# Exclude all .tfvars files, which are likely to contain sensitive data, such as
# password, private keys, and other secrets. These should not be part of version
# control as they are data points which are potentially sensitive and subject
# to change depending on the environment.
*.tfvars - любые файлы с расширением tfvars
*.tfvars.json любые файлы .tfvars.json

# Ignore override files as they are usually used to override resources locally and so
# are not checked in
# игонорим файлы:
override.tf
override.tf.json
# Игнорим все файлы 
*_override.tf
*_override.tf.json

# Include override files you do wish to add to version control using negated pattern
# !example_override.tf

# Include tfplan files to ignore the plan output of command: terraform plan -out=tfplan
# example: *tfplan*

# Ignore CLI configuration files
#Игнорим файлы:
.terraformrc
terraform.rc
