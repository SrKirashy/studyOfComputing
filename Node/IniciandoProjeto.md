# Inicio de Projeto
*Depois de criar um repositório para seu projeto, e clonar na sua máquina, insira o seguinte comando dentro do terminal do projeto:*
```
    npm init
```
*Dando esse comando o **package.json** sera criado.*

### Criando arquivo de configuração do Typescript:

*Inicie o arquivo de configuração do **Typescript** usando o seguinte comando:*

```
    tsc --init
```

#### Configure o Typescript:

*Nas configurações do **Ts**, descomente o **OutDir** e **RootDir**. O **OutDir** será a pasta **"dist"**, já o **RootDir** será a pasta **"src"**. Configure também o **"Target"**, para utilizar a versão mais recente do **ECMAScript**. E em seguida descomente o **"moduleResolution: node"** para o **Typescript** entender o tipo de projeto que está sendo trabalhado.*

# Instalando dependências

 **Instale todas dependências do projeto:**

 *Instale o **Express** juntamente com o **Mustache** ( que será usando como exemplo neste projeto que estamos iniciando, mas podem ser usadas outras **"template engines"** ), e o **dotenv** para usar as váriaveis de ambiente:*

 ```
    npm install express mustache-express dotenv
 ```

 **Instale todos @Types que serão utilizados no projeto:**

 *Após instalar as dependências, instale também os *Types* usando os seguintes comandos:*

 ```
    npm install --save-dev @types/express @types/mustache @types/node
 ```

 *O comando **"--save-dev"** fará com que os types sejam instalados apenas no ambiente de desenvolvimento, já que é o único lugar onde será utilizado.*

 *Você pode conferir todas as configurações no arquivo **"package.json"**.*

 ## Crie as pastas "src"

 *Crie a pasta **src** e dentro dela crie o arquivo **"server.ts"** ( onde terá as configurações do seu servidor. )*

---
 *Assumindo que você já tenha essas três denpedências instaladas **globalmente**:*
 ```
    1 - nodemon
    2 - typescript
    3 - ts-node
 ```

*Caso ainda não tenha, instale com o seguinte comando:*

```
    npm install -g nodemon typescript ts-node
```

*Vá até o **"package.json"** e em **"scripts"** crie um atalho para iniciar o projeto com mais facilidade.*

**Ex:**
```
    "scripts": {
        "start-dev": "nodemon -e ts,json,mustache src/server.ts"
    }
```

*Pronto! Agora é só configurar o seu arquivo **README.md** !*