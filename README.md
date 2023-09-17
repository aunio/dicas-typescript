# dicas-typescript

1.  [Pick](#pick)

## **Pick**

O pick permite criar um novo tipo baseado em um já existente, mas selecionando apenas as propriedades que queremos.

```javascript
type Usuario = {
  name: string,
  age: number,
  email: string,
};

type SemEmail = Pick<Pessoa, "name" | "age">;

const usuarioSemEmail: UsuarioSemEmail = {
  name: "Aunio",
  age: 32,
};
```

**[⬆ Voltar para o início](#dicas-typescript)**
