# Configurando server.ts

*Importe tudo que será usado:*

```
    import express from 'express';
    import dotenv from 'dotenv';
    import mustache from 'mustache-express';
    import path from 'path';
```

## Configure a váriavel de ambiente

*Crie uma pasta chamada **.env** e dentro dela coloque o comando **"PORT=-porta que você quer utilizar-"***

*Agora dentro do **server.ts** insira o comando:*

```
    dotenv.config();
```

## Configure o servidor

*Insira o código:*

```
    const server = express();
```

### Configure o template engine

*Declare qual **engine** está sendo utilizada:*

```
    server.set('view engine', 'mustache');
```

*Insira onde será a pasta de vizualização do projeto, exemplo:*

```
    server.set('views', path.join(__dirname, 'views'));
```

*Não esqueça de criar a pasta **'views'** dentro da **'src'**.*

*E por final, set a **engine mustache**:*
```
    server.engine('mustache', mustache());
```

### Configure a pasta pública

*Crie a pasta **"public"**, onde ficarão o css, imagens e outros detalhes do projeto.*

### Use o servidor

*Use o servidor inserindo no arquivo **server.ts** o código:*

```
    server.use(express.static(path.join(__dirname,'../public')));
```

### Rodando servidor

*Após inserir as rotas, coloque o servidor para rodar:*

```
    server.listen(process.env.PORT);
```

# Visão geral da configuração do server.ts

*Configuramos as váriaveis de ambiente com o **dotenv**, o próprio servidor express configurado juntamente com o mustache setado, e nossa página estática também configurada para rodar.*

**Visão geral:**
```
    import express from 'express';
    import dotenv from 'dotenv';
    import mustache from 'mustache-express';
    import path from 'path';

    dotenv.config();

    const server = express();

    server.set('view engine', 'mustache');
    server.set('views', path.join(__dirname, 'views'));
    server.set('mustache', mustache());

    server.use(express.static(path.join(__dirname,'../public')));

    // Rotas

    server.listen(process.env.PORT);

```