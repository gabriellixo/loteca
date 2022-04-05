# Projeto Loteca
Este é um projeto de simulador de loteria, onde o usuário digita 6 números e realiza o sorteio de outros no final é verificado
quantos números ele acertou

## Tecnologias utilizadas
- **HTML** : estrutura do site
- __CSS__ : estilização do site
- *_JS_* : funções do site
- ~~BootStrap~~ : não foi utilizado



### Melhorias Possiveis
1. [x] Subir para GitHubPages
2. [ ] Alterar os Alerts
3. [ ] Utilizar o BootStrap
4. [ ] Deixar responsivo

### disponibilizado em
[GitHubPage](https://ruegab.github.io/loteca/)


### Prints da tela

| ID | Primeira Tela | Segunda Tela |
|----|---------------|----------------|
|  1 | loteca limpa  | loteca preenchida |
| 2  | ![tela loteca não preenchida](https://user-images.githubusercontent.com/100212761/161781610-06298240-1dd9-46b7-848a-96ffa21bb8c2.png) | ![tea preenchida](https://user-images.githubusercontent.com/100212761/161782415-91bf5624-ad97-435b-9187-af9ff3e95c41.png)|


#### Função Principal
```js:
function sorteioNum(){
    if(numDig.length < 6){
        alert("Antes de sortear digite 6 numeros nos campos")
        
    numSort=[]
    do{
        let sort = Math.ceil(Math.random()*60)        
        if(!numSort.includes(sort))
            numSort.push(sort) 

    }while(numSort.length<6)

    document.getElementById("numsort").innerHTML=numSort
    verificaAcertos()
    }else{
        alert("aprovada na disciplina do carlos");
    }

}
```

#### comando git
para iniciar o projeto
```bash:
git init
```

