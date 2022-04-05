# projeto loteca

este é um proeto de um simulador de loteca, onde o usuario digita 6 numeros e realiza um sorteio de outros 6 numeros
no final é verificado quantos numeros ele acertou

## tecnologoas utilizadas

- **HTML**; estrutura do site
- __CSS__; estilização do site
- *_JS_*; funções do site
- ~Bootstrap~; Não foi utilizado

### Melhorias possiveis

1. [ ] Subir para GitHubPages
2. [ ] Alterar os Alerts
3. [ ] Utilizar Bootstrap
4. [ ] Deixar responsivo

### disponibilizado em 
[GithubPages](https://gabriellixo.github.io/loteca/)

### Prints de tela

| ID | Primeira tela | Segunda tela |
|----|---------------|----------------|
| 1 | Loteca limpa | Loteca preenchida |
| 2 | ![tela loteca não preenchida](https://user-images.githubusercontent.com/100213322/161781602-f3cc1e93-94a4-4f81-97a7-8669965d1cce.png)
| 3 | ![tela loteca preenchida com sortear](https://user-images.githubusercontent.com/100213322/161782405-0dc2a39f-07b0-48be-8bcf-effb2dab9917.png)

### Função Principal

```
function sorteioNum(){
    if(numDig.length < 6){
        alert("Antes de sortear digite 6 numeros nos campos")
    } else {
        
    numSort=[]
    do{
        let sort = Math.ceil(Math.random()*60)        
        if(!numSort.includes(sort))
            numSort.push(sort) 

    }while(numSort.length<6)

    document.getElementById("numsort").innerHTML=numSort
    verificaAcertos()
    }
```

#### comando git
para iniciar projeto
``` bash:
git  init
```
