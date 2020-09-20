# Golang Nepal site powered by hugo

This repo contains the source code for the golang nepal site golangnepal.github.io 

The hugo generated public static code is saved in the other repo https://github.com/GolangNepal/golangnepal.github.io . This repo `GolangNepal/golangnepal.github.io` is auto generated from this repo.

git Sub module is used to push the code to golangnepal.github.io. Any thing changed is this repo will generate generated in the public folder. This public folder is a sub module for the `GolangNepal/golangnepal.github.io` repo. So after changing things here, you can simply push the code. To push the code in both repo use the following command:

```
./deploy.sh
```

For more details on how to host a hugo site to github here is a article https://gohugo.io/hosting-and-deployment/hosting-on-github/
