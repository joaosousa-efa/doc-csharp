## Após instalar .Net 8 no Linux

Adicionar ao .bashrc (para uma instalação manual)

```
# microsoft dot net
#export PATH=$PATH:$HOME/dotnet
#export DOTNET_ROOT=$HOME/dotnet
```
Criar o projecto

```
dotnet new console --name <nome-projecto>
```

Para testar
```
dotnet run
```

Para publicar
```
dotnet publish
```
Precisa de ter o .NET runtime instalado para rodar o executável 

Publicar sem o runtime para uma plataforma específica (tamanho é um pouco maior)

```
dotnet publish -r linux-x64
dotnet publish -r win-x64
```

Publicar com o runtime incluido (cerca de 150 Mb)
```
dotnet publish --self-contained
```

Instalar pacote
```
dotnet add package <nomePacote> --version 1.0
```


## Blazor

```
dotnet new blazor -o <BlazorNomeApp>
```

Abrir ambiente de desenvilvimento

```
cd <BlazorNomeApp>
code .
dotnet watch
```


