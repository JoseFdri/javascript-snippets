# javascript-snippets
Snippets for Javascript

#Poner comas a un numero
```
var poner_comas = function (numero) {
    numero += ''
    var posPunto = numero.indexOf('.')
    var final = []
    var contador = 0
    for (var i = numero.length -1; i >= 0 ; i--) {
      final.push(numero[i])
      if(i < posPunto) {
        contador++
        if(contador % 3 == 0 && i > 0) {
          final.push(',')
        }
      }
    }
    return final.reverse().join('')
  }
  ```
