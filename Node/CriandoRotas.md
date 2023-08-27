# Criando Rotas

*Crie a pasta **'routes'** dentro de **'src'** e configure as rotas, importando Router:*

```
    import Router from 'express';

    const router = Router();

    // Configure aqui as rotas!
    // Ex:
    //
    //  router.get('/', (req, res) => {
    //  res.send('home');
    //  })



    export default router;
```

*Em **"server.ts"** importe as rotas que você irá utilizar:*

```
    import mainRoutes from "./routes/index"
```
*E use elas:*

```
    server.use(mainRouts);
```

*Crie também a posibilidade de não funcionar:*

```
    server.use((req, res)=>{
        res.send('Página não encontrada!')
    })
```