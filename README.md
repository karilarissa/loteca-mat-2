# Projeto Loteca
Este é um projeto de simulador de loteria, onde o usuário digita 6 números e realiza o sorteio de outros no final é verificado quantos números ele acertou

## Tecnologias utilizadas
- **HTML**: estrutura do site
- __CSS__: estilização do site
- *_JS_*: funções do site
- ~~BootStrap~~: não foi utilizado 


### Melhorias Possíveis
1. [X] Subir para GitHubPages
2. [ ] Alterar os Alertas
3. [ ] Utilizar o BootStrap
4. [ ] Deixar Responsivo

### disponibilizado em
[GitHubPage](https://karilarissa.github.io/loteca_mat/)

### Prints da tela

| ID | Primera tela | Segunda tela |
|----|---------------|---------------|
| 1  | loteca limpa | loteca Preenchida |
| 2  | ![tela loteca não preenchida](https://user-images.githubusercontent.com/101194427/161782747-adef7aae-4ac2-436c-97c0-6c702b2ef318.png) | ![image](https://user-images.githubusercontent.com/101194427/161782453-c1ceec2e-fc77-47f2-8de9-a04a677d0505.png) |


#### Função Principal
```js:
function sorteioNum(){
  if(numDig.length < 6){
    alert("Antes de sortear digite 6 números nos campos")

  numSort=[]
  do{
    let sort = Math.ceil(Math.random()*60)
    if(!numSort.includes(sort))
        numSort.push(sort)
  }while(numSort.length<6){

    document.getElementById("numsort").innerHTML=numSort
    verificaAcertos()
  }else{
    alert("Aprovada!")
  }
  }
}

```

#### comando git
para iniciar o projeto
```bash:
git init 
```
