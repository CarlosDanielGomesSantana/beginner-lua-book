# Comentários

Comentários são úteis para quem e escreve o código em qualquer linguagem. Em Lua, isso não é diferente, mas para quem veio de outras linguagens verá o quanto é poderoso esse recurso.

> Lembre-se que os comentários **_não são lidos pela linguagem_** na hora de executar seus códigos.

## Comentários de uma linha

Comentários de uma linha são simples, mas ajudam a descrever rápido e fácil um trecho de código que seja pequeno. Como por exemplo falar o que determinada linha abaixo ou trecho faz.

```Lua
-- Esse código abaixo imprime uma mensagem
print('Acima dessa linha existe um comentário')
```

## Comentários de múltiplas linhas

Comentários de múltiplas linha servem para descrever até mais que apenas um comportamento de um trecho simples de código, mas serve para documentar uma função, um módulo, uma table, etc.

```Lua
--[[
    Autor: Carlos D. G. Santana
    Descrição: É um exemplo de comentários em múltiplas linhas
]]
print('Existe várias linhas de comentários acima de mim')
```

## Habilitar e desabilitar código

Após aprender o que são os comentários de única e múltiplas linhas. Veremos comentários que desabilitam e habilitam código. Esse conceito não é visto em outras linguagens, mas existem uma grande utilidade na hora de testar trechos de código.

```Lua
---[[
print('esse código está desabilitado')
--]]

--[[
print('esse código está desabilitado')
--]]
```

### Por quê isso acontece?

Observe que há uma diferença entre **"--[["** e **"---[["** (uma tem 2 "-" e a outra 3 **"-"**).

Em **"--[["**, é apenas o comentário de multiplas linhas, ou seja, o que estiver entre o início de **"--[["** e no fim de **"--]]"** será ignorado pela linguagem.

Contudo, em **"---[["** transformamos com o **"-"** a mais em comentário de uma linha e como no final existe **"--]]"** que também é um comentário de uma linha. Então, temos tudo que está entre **"---[["** e **"--]]"**

```Lua
--[[ Comentário de múltiplas linhas
print('Olá Mundo!')
--]]

---[[ Comentário de uma linha
print('Olá Mundo!')
--]] Comentário de uma linha
```
