# dicas-typescript

1.  [Omit](#omit)
1.  [Pick](#pick)

## **Omit**

O omit permite criar um novo tipo a partir de um já existente, mas excluindo as propriedades que não queremos.

```javascript
type Usuario = {
  nome: string,
  idade: number,
  email: string,
};

type UsuarioSemEmail = Omit<Pessoa, "email">;

const usuario: Usuario = {
  nome: "Maria",
  idade: "30",
  email: "maria@email.com",
};

const usuarioSemEmail: UsuarioSemEmail = {
  nome: "Maria",
  idade: "30",
};
```

## **Pick**

O pick permite criar um novo tipo a partir de um já existente, mas selecionando apenas as propriedades que queremos.

```javascript
type Usuario = {
  nome: string,
  idade: number,
  email: string,
};

type SemEmail = Pick<Pessoa, "nome" | "idade">;

const usuario: Usuario = {
  nome: "Maria",
  idade: "30",
  email: "maria@email.com",
};

const usuarioSemEmail: UsuarioSemEmail = {
  nome: "Maria",
  idade: "30",
};
```

**[⬆ Voltar para o início](#dicas-typescript)**
