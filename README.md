# appstarter

## Instalação
Clonar este repositório:
Dentro do diretório `www` do Laragon, digite o seguinte comando:
```
git clone git@github.com:rahpt/ci4-appstarter.git
```

Após instalar, corra o migration para criar as tabelas
```
spark migrate --all
```
crie o utilizador ADMIN

spark shield:user create -n Admin -e admin@admin.com

adicione em um grupo admin
 spark shield:user addgroup -n Admin -g admin

ativa o usuario
spark shield:activate -n Admin

git tag -a 1.0.0.0 -m "V 1.0.0.0"

git push origin 1.0.0.0