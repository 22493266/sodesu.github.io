## Env
- install terraform in your local PC
- install AWS CLI tools on your local PC
- intialize the AWS env

## Get Start
- create terraform script (XXX.tf)
- to inti the local terraform with ``` terraform init ```
- to format the .tf script with ``` terraform fmt ```
- to validate the .tf script with ``` terraform validate ```
- to build the project with  ``` terraform apply ```
- to show the project state with ``` terraform state list ```

## Variable
### Separeted .tf file
- new variable.tf
```
variable "instance_name" {
  description = "Value of the Name tag for the EC2 instance"
  type        = string
  default     = "ExampleAppServerInstance"
}
```
- to use the variable(s)
```
...
   tags = {
-    Name = "ExampleAppServerInstance"
+    Name = var.instance_name
   }
...
```

### From the command line
set the variable from command line like this:
``` $terraform apply -var "instance_name=YetAnotherName" ```


