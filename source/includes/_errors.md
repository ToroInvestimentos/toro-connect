## Erros

Ao requisitar o id_token, alguns erros podem ocorrer. Abaixo segue o layout de como o erro é retornado do provedor de autenticação Toro.

### layout do erro

```json
{
    "error": "unauthorized_client",
    "error_description": "requested grant type is not allowed for this client"
}
```

Um erro pode acontecer se algum parametro passado, como um response_type, for diferente do cadastrado no Toro Connect. Nesse caso, o layout da resposta é composto por uma propriedade chamada <code>error</code> e outra chamada <code>error_description</code>, que seria o nome do erro e sua descrição, respectivamente.

Exemplo ao lado.