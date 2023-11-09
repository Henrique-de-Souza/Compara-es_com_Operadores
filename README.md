# Desafio 🥇 Aula 4 - Dev Aprender

### Enuciado:
Quero que você defina as seguintes variáveis, inicialmente todas como False, a ideia aqui não é de se importar com os valores dentro dessas variáveis, mas sim como montar condicionais.

```ruby
possui_passaporte = False

passagem_comprada = False

menor_de_idade = False
```

### OBS: Antes de tudo, fiz um input para o resultado ficar mais dinânico

```ruby
nome = str(input('Digite seu nome: '))
```

###  E Crie as seguintes condições usando o que acabou de ver e imprima o resultado na tela. Tente fazer cada condição e depois veja a solução no final deste aula.
1 - Uma pessoa só pode viajar se possuir passaporte e tiver a passagem comprada e não for menor de idade

```ruby
# 1º caso:
if (possui_passaporte==True and passagem_comprada==True) and menor_de_idade==False:
    print(f'Tudo ok {nome}! Você pode viajar!')
else:
    print(f'Poxa {nome}! Você não poderá viajar')
```

2 - Uma pessoa só pode viajar se possuir passaporte ou tiver a passagem comprada e não for menor de idade

```ruby
# 2º caso:
if (possui_passaporte==True) or (passagem_comprada==True and menor_de_idade==False):
     print(f'Tudo ok {nome}!Você pode viajar!')
else:
    print(f'Poxa {nome}! Você não poderá viajar')
```

3 - Uma pessoa só pode viajar se não possuir passaporte ou tiver a passagem comprada e não for menor de idade

```ruby
# 3º caso:
if (possui_passaporte==False or passagem_comprada==True) and menor_de_idade==False:
      print(f'Tudo ok {nome}! Você pode viajar!')
else:
    print(f'Poxa {nome}! Você não poderá viajar')
```

4 - Uma pessoa não pode viajar se não possuir passaporte ou não tiver a passagem comprada e for menor de idade

````ruby
# 4º caso:
if (False or False) and True:
     print(f'{nome}! Sinto muito, mas você não poderá viajar hoje')
else:
    print(f'Tudo ok {nome}! Você pode viajar')
````


### Código completo

```ruby
possui_passaporte = False

passagem_comprada = False

menor_de_idade = False

nome = str(input('Digite seu nome: '))

# 1º caso:
if (possui_passaporte==True and passagem_comprada==True) and menor_de_idade==False:
    print(f'Tudo ok {nome}! Você pode viajar!')
else:
    print(f'Poxa {nome}! Você não poderá viajar')

# 2º caso:
if (possui_passaporte==True) or (passagem_comprada==True and menor_de_idade==False):
     print(f'Tudo ok {nome}!Você pode viajar!')
else:
    print(f'Poxa {nome}! Você não poderá viajar')

# 3º caso:
if (possui_passaporte==False or passagem_comprada==True) and menor_de_idade==False:
      print(f'Tudo ok {nome}! Você pode viajar!')
else:
    print(f'Poxa {nome}! Você não poderá viajar')

# 4º caso:
if (False or False) and True:
     print(f'{nome}! Sinto muito, mas você não poderá viajar hoje')
else:
    print(f'Tudo ok {nome}! Você pode viajar')
    

```

